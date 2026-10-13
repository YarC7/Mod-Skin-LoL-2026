# Note vận hành định kỳ

## Mỗi patch LoL (~2 tuần)

- [ ] **Skin mới:** C:\Users\Cankkun\projects\desktop\my-app\new-resource\LeagueSkins => git pull ở đây
- [ ] **Patcher hết hạn?** Mở app → Settings → mode Auto: nếu `patcher: HẾT HẠN` → update LTK Manager → copy đè 2 file (`ltk_patcher_host.exe`, dll) nếu chơi portable.
- [ ] **Data DDragon:** `node scripts/fetch-ddragon-data.mjs` khi có tướng/skin mới → commit JSON. Script tự gen cả `champion_key_map.json` từ DDragon (khỏi soi `skin_ids.json` tay) và đối chiếu chéo với folder `skins/` local — có dòng `league-skins missing` hay `unknown champKey` là lệch, xử lý rồi chạy lại.

## Khi cần release bản mới

```powershell
git add -A; git commit -m "..."
git push origin main; git tag vX.Y.Z; git push origin vX.Y.Z
```

Workflow `publish.yml` tự build + đăng Releases. Máy khác cài bản mới là có fix.

## Không cần đụng tới

- `mod-tools.exe` — đóng băng, bundle sẵn trong `tools/`.
- `.git` của mirror `D:\LeagueSkins` — clone `--depth 1` từ đầu thì nhẹ; phình thì xóa clone lại.
- CDN/bot-filter — đã allow UA app + Node; chỉ check khi đổi domain.


tóm lại là 
C:\Users\Cankkun\projects\desktop\my-app\new-resource\LeagueSkins => git pull
node scripts/fetch-ddragon-data.mjs
node scripts/upload-skins-r2.mjs
nâng version package json
git add -A
git commit -m "..."
git tag vX.Y.Z
git push origin main
git push origin vX.Y.Z
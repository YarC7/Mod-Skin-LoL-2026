# Đóng góp cho Mod Skin LoL

Cảm ơn bạn đã quan tâm! Mọi PR, báo lỗi, góp ý đều được chào đón.

## Chạy dev

```powershell
npm install
npm start    # chạy dev
npm run lint # kiểm tra eslint
npm run make # đóng gói thử (x64)
```

## Quy trình PR

1. Fork repo, tạo nhánh từ `main` (`feat/...`, `fix/...`).
2. Code + test thủ công flow Apply skin (mode LTK Manager và Auto nếu đụng engine).
3. PR vào `main`, mô tả rõ: làm gì, test thế nào, ảnh chụp nếu đổi UI.

## Release (maintainer)

```powershell
git add -A; git commit -m "..."
git push origin main; git tag vX.Y.Z; git push origin vX.Y.Z
```

Workflow `publish.yml` tự build + đăng Releases khi push tag `v*.*.*`.

## Lưu ý

- Đừng commit `.env`, `node_modules`, folder `new-resource/`, file `.fantome` lẻ.
- Tool bundle trong `tools/` (GPL cslol) chỉ update khi có bản mod-tools mới đã verify.
- Data DDragon: chạy `node scripts/fetch-ddragon-data.mjs` rồi commit JSON.

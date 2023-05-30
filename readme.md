## Các câu lệnh git hay dùng

```
1. git pull remote-name branch-name (Kéo code của 1 branch từ một remote dự án)
2. git add file-name-1 file-name-2 (Add file changes before a commit)
3. git commit -m "Tên commit" (Tạo một commit mới)
4. git push remote-name branch-name (Đẩy code lên một remote dự án)
```

## Tạo một pull request

```
1. Click to pull request in github
2. Click to create pull request
3. Chooose branch base want create pull (Default is master)
4. Chooose branch want merge to branch base
```

## Cấu trúc folder react tối ưu và hay được sử dụng

```
src/
├── assets/ {/* lưu ảnh cứng của page thì bỏ vào đây :v */}
├── components/
│   ├── compound/ {/* gộp các components từ `primitive` tại đây */}
│   │   ├── GroupInput.jsx
│   │   └── GroupSearch.jsx
│   └── primitive/ {/* build các common button/component nhỏ lẽ */}
│   │   ├── Input.jsx
│   │   └── Search.jsx
├── hooks {/* xây dựng các function với hooks */}
├── i18n {/* xử lý đa ngôn ngữ */}
├── layout {/* nơi build layout cho page để dùng chung */}
│   ├── Header/
│   │   └── index.jsx
│   └── Footer/
│   │   └── index.jsx
├── pages {/* xử lý các màn tại đây */}
│   ├── home/ {/* import các layouts, compound, primitive để handle pages */}
│   │   └── index.jsx
│   |   |   ├── HomeItem/ {/* nếu có các màn con thì tạo ntn */}
│   |   |   |   └── index.jsx
│   |   |   └── HomeSearch/
│   |   |   |   └── index.jsx
│   └── 404/
│   │   └── index.jsx
├── scss
│   ├── abstracts/ {/* config bộ khung scss */}
│   ├── base/ {/* cofig biến global */}
│   ├── components/ -> pages/  {/* nơi viết css cho các components tương ứng */}
│   └── utils/ {/* các helper css dùng chung */}
├── services {/* chứa các module/service được sử dụng để tương tác với API */}
├── store {/* là nơi quản lý store/state cho redux saga, mn đọc thêm ở code nhé */}
├── svg {/* dùng để chưa các file hoặc Icon svg */}
├── ultis {/* nơi viết các constants, helper common */}
└── validates {/* xử lý validation */}
```

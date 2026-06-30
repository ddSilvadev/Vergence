# Vergence
Synchronize, edit, and publish multi-perspective videos from livestream VODs.



vergence/
│
├── engine/
│   ├── editing/
│   ├── timeline/
│   ├── retrieval/
│   ├── rendering/
│   ├── synchronization/
│   ├── upload/
│   └── ai/
│
├── workers/
│   ├── download.py
│   ├── render.py
│   ├── upload.py
│   └── thumbnails.py
│
├── api/
│
├── cli/
│
├── web/
│
├── desktop/
│
├── docs/
│
└── tests/
```



The reason I like this is that if someone lands on your repository six months from now, they can immediately understand the system:

- **engine** = business logic
- **workers** = asynchronous execution
- **api** = HTTP interface
- **cli** = power-user/prototyping interface
- **web/desktop** = clients
# 2024-04-08-build-rag-with-typescript

[![Watch the video](https://img.youtube.com/vi/8rz9axIzIy4/maxresdefault.jpg)](https://youtu.be/8rz9axIzIy4)

- [install bun](https://bun.sh/docs/installation) `bun`: `npm install -g bun`
- [install chromadb](https://docs.trychroma.com/getting-started?lang=js#1-install) chromadb backend: `pip install chromadb`
- cd into project directory :`cd technovangelist-videoprojects/2024-04-08-build-rag-with-typescript`
- configure `config.json`
- Install dependencies: `bun install`.
- Run Chroma on a separate terminal: `chroma run --host localhost --port 8000 --path ../vectordb-stores/chromadb`
- Run chromadb with telemetry disabled:
	- `ANONYMIZED_TELEMETRY=False chroma run --host localhost --port 8000 --path ../vectordb-stores/chromadb`
- Run import: `bun import.ts `
- Run search: `bun search.ts What happened in Taiwan?`

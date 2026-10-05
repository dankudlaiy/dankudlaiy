### danylo kudlai

software engineer. backend systems in .net and applied ai, building for us product teams since 2022.

**work**

- **real-estate platform rebuild** (us product, ~10 engineers): azure monolith → .net 10, postgresql, next.js and temporal on aws. second-largest contributor.
  - bootstrapped the new backend: clean architecture, cqrs, jwt + rbac.
  - wrote a deterministic offer-pricing library.
  - built a property-data aggregator that queries three vendors in parallel and keeps per-field provenance, verified against the legacy system with a live differential harness.
  - built the underwriting app end to end.
  - replaced a mongodb + elasticsearch + rabbitmq service with a library over postgres and removed its infrastructure in terraform.
- **real-time speech-to-speech call translator** (freelance): live sip calls, russian → german in a cloned voice, used by a call-centre client's operator.
  - stack on one gpu: pjsip bridge, fastapi + websockets, streaming asr (gigaam, parakeet, faster-whisper), a 30b moe translation model on llama.cpp, qwen3-tts on vllm.
  - distilled a simultaneous-interpretation policy into lora adapters from synthetic, llm-labelled calls; ~50 evaluation modules.
- **multi-tenant ai assistant backend**: knowledge bases, document-ingestion workflows on temporal, chat api. .net 8, postgresql, kubernetes.
- **vehicle-auction marketplace for credit unions**: .net 6 on azure (functions, cosmos db, service bus), identityserver4 sign-in, partner integrations.
- **call-centre analytics and dialer** (freelance): real-time call tracking from asterisk ami/ari events. .net 8, blazor, signalr, postgresql.

**research and side projects**

- **game-theory engine for imperfect-information games:**
  - cfr solvers on gpu, exploitability checks (local best response), aivat variance reduction;
  - bayesian opponent modelling on ~400k decisions, paired-seed a/b simulator;
  - vlm screen reading on vllm, retrieval with sentence-transformers + chromadb.
  - python, rust.
- **rag pipelines** in my own projects: embeddings, chunking and retrieval with sentence-transformers, chromadb, faiss.
- **multi-agent pipeline**: role-based llm agents (director, designer, programmer, artist) with scoped write permissions and review gates.
- [**agent-workflow**](https://github.com/dankudlaiy/agent-workflow): claude code team setup for .net / next.js repos. spec → plan → test-first → legacy parity → review, enforced by hooks.
- [**iko**](https://github.com/dankudlaiy/iko): one playlist across spotify, youtube and apple music. asp.net core 8, angular 20, oauth 2.0, integration tests, docker.
- [**tiler**](https://github.com/dankudlaiy/tiler): drag-to-tile window manager for windows. .net 10, wpf, win32 interop, unit-tested layout engine.

**stack**

- **backend:** c#, .net 6–10, asp.net core, ef core, postgresql, sql server, cosmos db, redis, rabbitmq, temporal
- **cloud:** aws, azure, terraform, docker, kubernetes, github actions
- **frontend:** typescript, react, next.js, angular
- **ai:** python, fastapi, vllm, llama.cpp, whisper, lora, rag, mcp

[linkedin](https://www.linkedin.com/in/danylo-kudlai) · dankudlaiy@gmail.com

<sub>bsc computer science, university of łódź · microsoft azure developer associate (az-204) · databricks data engineer associate</sub>

# Router-Lib

[![CI](https://github.com/kapildhinwa2010-dev/Router-Lib/actions/workflows/ci.yml/badge.svg)](https://github.com/kapildhinwa2010-dev/Router-Lib/actions/workflows/ci.yml)
[![CodeQL](https://github.com/kapildhinwa2010-dev/Router-Lib/actions/workflows/codeql.yml/badge.svg)](https://github.com/kapildhinwa2010-dev/Router-Lib/actions/workflows/codeql.yml)

Complexity-based request routing.

**Part of the [Kapildhinwa2010-dev Toolkit](https://github.com/kapildhinwa2010-dev/Kapildhinwa2010-dev).**

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- Composite complexity score (norm + normalized entropy)
- Cheapest-sufficient-expert routing
- Per-expert usage reports

## 📦 Install

```bash
pip install -r requirements.txt
```

## 🚀 Quick start

```python
from router_lib import ComplexityRouter

router = ComplexityRouter()
router.add_expert('tiny', capacity=1.0, cost=0.1)
router.add_expert('big', capacity=100.0, cost=10.0)
print(router.route_and_handle(x))
```

## 🧪 Tests

```bash
pytest tests/ -v
```

## 📄 License

MIT — see [LICENSE](LICENSE).

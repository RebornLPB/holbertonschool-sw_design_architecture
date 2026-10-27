# Software Design - Design Patterns

## Description
This project implements three classic Gang-of-Four design patterns in Python: the **Factory** pattern to create objects through a registry instead of direct instantiation, the **Observer** pattern to broadcast topic-based notifications to subscribers, and the **Decorator** pattern to dynamically add pricing/description behaviour to a beverage.

All scripts are written for **Python 3.8+** and follow the **PEP 8** style guide.

## 📝 Learning Objectives
* Implement the **Factory** pattern with a registry (`dict`) mapping names to classes, allowing new types to be registered at runtime.
* Implement the **Observer** pattern with a `Protocol`, per-observer topic filtering, and a `notify()` broadcast.
* Implement the **Decorator** pattern by wrapping an abstract base class (`Beverage`) so behaviours can be composed (`MilkDecorator`, `SugarDecorator`, `CaramelDecorator`).
* Recognize when each pattern is the appropriate tool for a design problem.

## 🛠️ Requirements & Engineering Constraints
* **OS:** Ubuntu 20.04 LTS
* **Interpreter:** `python3` (version 3.8.5+)
* **Style Guide:** Code is meant to follow the PEP 8 style guide.

## 📁 File List & Tasks Directory

| File | Task Title | Description |
| :--- | :--- | :--- |
| `0-factory.py` | Factory Pattern | `VehicleFactory` creates `Bus`, `Train`, `Bike`, and a dynamically-registered `Scooter` through `create(kind)` / `register_kind(name, cls)`. |
| `1-observer.py` | Observer Pattern | `NewsSubject` lets observers `subscribe`/`unsubscribe` to specific topics (or all); `LogObserver`, `EmailObserver`, and `SmsObserver` react to `notify(topic, data)`. |
| `2-decorator.py` | Decorator Pattern | `Beverage` (abstract) is wrapped by `MilkDecorator`, `SugarDecorator`, and `CaramelDecorator`, each adding to `cost()` and `description()`. |

---

## 🚀 Execution

```bash
python3 0-factory.py
python3 1-observer.py
python3 2-decorator.py
```

---

## 👤 Author
* **Student:** [RebornLPB](https://github.com/RebornLPB)
* **GitHub:** [https://github.com/RebornLPB](https://github.com/RebornLPB)
* **School:** [Holberton School](https://www.holbertonschool.com/)

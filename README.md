# react-cryon

A lightweight engine for predictive microservice orchestration based on event feedback.

### Setup

Requires Python 3.8+.

```bash
pip install react-cryon
```

### Usage

```python
from reactcryon import Orchestrator

# Initialize engine
engine = Orchestrator(model_path="predict.pkl")

# Register service and predictive trigger
engine.register("auth-service", threshold=0.85)

# Trigger evaluation
engine.pulse("auth-service", telemetry_data)
```

### Testing

Run the test suite to verify internal logic:

```bash
python3 test_reactcryon.py
```

### License

MIT License.



---
Sidebar_Label: default_planning_agent
Title: portia.planning_agents.default_planning_agent
---

DefaultPlanningAgent is a single best effort attempt at planning based on the given query + tools.

## DefaultPlanningAgent Objects

```python
class DefaultPlanningAgent(BasePlanningAgent)
```

DefaultPlanningAgent class.

#### \_\_init\_\_

```python
def __init__(config: Config) -> None
```

Init with the config.

#### generate\_steps\_or\_error

```python
def generate_steps_or_error(
        query: str,
        tool_list: list[Tool],
        end_user: EndUser,
        examples: list[Plan] | None = None,
        plan_inputs: list[PlanInput] | None = None) -> StepsOrError
```

Generate a plan or error using an LLM from a query and a list of tools.


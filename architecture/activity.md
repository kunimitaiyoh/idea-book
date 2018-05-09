# Activity

`Activity` that refers Activity in Android is blueprint that represents
how components should behavior on each corresponding router on single page apllications.

## Actions and states

### global actions and states

- `activities`
    - `stack` in `stacks`: contains context of each Acitivity instance.
        - `state`: local state of the activity.
        - `activity`: indicates which activity should be used for restarting. (optional)

### local actions and states

- `back()`: close the active activity and back to previous one.
- `start(activity: Activity)`: start new Activity. this may cause destroying old activities or not.

#### lifecycle hooks

- `oncreate()`: called when the activity is instantiated.
- `onresume()`: called when user returns to the activity.
- `onpause()`: called when the activity is no longer visible.

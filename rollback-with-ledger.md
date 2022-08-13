## How To Rollback With Ledger

<span style="color:red">**WARNING: Highly Technical Nonsense Ahead!**</span>

If you're a regular user, this doesn't concern you.

To undo player actions with ledger, you use the command /ledger rollback <params>. To preview a rollback, run /ledger preview rollback <params>.

### Parameters:
  - action
    - Type of player action to rollback. Valid actions:
        - block-break
        - block-place
        - block-change
        - item-insert
        - item-remove
        - entity-killed
  - range
    - Selects an area to rollback in across all dimensions
  - world
    - Selects an entire dimension to perform a rollback in
  - object
    - Filters by block/item/entity type broken/placed/changed/inserted/removed/killed
  - before
    - Selects actions from before the point in time that was provided. Example: before:1d selects all actions that occurred before yesterday
  - after
    - Selects actions from after the point in time that was provided. Example: after:1d selects all actions that occurred after yesterday
  
### Example Commands
  /ledger rollback action:block-break after:1d world:minecraft:overworld source:Player123 - This command replaces every block broken by player Player123 after yesterday in the overworld

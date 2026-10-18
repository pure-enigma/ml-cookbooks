# modular_dl_models

Build models as compositions of pure blocks to keep the code readable. A block is self-contained, with explicit inputs and outputs and no hidden or global state, and is itself built from other blocks. Imported components, such as a transformer, are blocks; when modifying one, create a new block rather than editing it inline. The top-level model only wires blocks together; logic lives in blocks.

Keep `<model-arch>` as the living view of the final model: its blocks, how they connect, and key shapes, with a diagram where it helps. Update it whenever the model's composition changes. It shows what the model is now, not what we tried.

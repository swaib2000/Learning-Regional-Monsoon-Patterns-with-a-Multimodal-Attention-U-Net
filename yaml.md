
All actual data files are hosted on Hugging Face.

---

## 📦 Accessing the Dataset

### 👉 Hugging Face Dataset Page
https://huggingface.co/datasets/swaib/Multimodal_Monsoon_Indian_Dataset

You can browse files, download individual states, or clone the full dataset.

### Example: Download Using `huggingface_hub`

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="swaib/Multimodal_Monsoon_Indian_Dataset",
    repo_type="dataset",
    local_dir="monsoon_dataset"
)

# Human Feedback in Enhancing Image Generation Models with Direct Preference Optimization

## Usage
- Install the necessary libraries:
```bash
git clone https://github.com/bdbao/hfsd-pap
cd hfsd-pap
pip install -e .
```
- Download dataset:
  (We use Kvasir-SEG for inpainting task)
```bash
bash train_data/dataset.sh
```
- Sampling and Training process:
  - Sample:
    ```bash
    accelerate launch scripts/sample_inp.py
    ``` 
  - UI for human feedback phase:
    ```bash
    python ui/human_feedback.py
    ``` 
  - Train:
    ```bash
    accelerate launch scripts/train_inp.py
    ``` 

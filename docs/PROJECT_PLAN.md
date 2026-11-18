# Project plan and reproducibility checklist

This plan is a roadmap. A task should be marked complete only when supported by files or reproducible evidence in this repository. The supplied academic report informs the documented project scope, but report statements alone do not verify implementation or results.

## 1. Add implementation and provenance

- [ ] Add the actual source code or notebook used for the traffic-sign project.
- [ ] Record the YOLOv5 variant, upstream repository revision, modifications, and attribution.
- [ ] Confirm whether the trained model uses pretrained weights; record checkpoint filename, source, checksum, and usage terms.
- [ ] Record Python, PyTorch, Ultralytics/YOLOv5, OpenCV, NumPy, and other dependency versions from the working environment.
- [ ] Provide a tested dependency manifest and setup steps for development and Raspberry Pi OS.
- [ ] Document supported hardware, camera, display, and any non-default system configuration.

## 2. Document data and task

- [ ] Verify the Roboflow `road-signs-6ih4y` dataset version and its terms of use.
- [ ] Record all 17 class names, annotation format, image dimensions, and data preparation steps.
- [ ] Document exact training, validation, and test split sizes and how the splits were created.
- [ ] Record augmentation and preprocessing settings from the actual configuration.
- [ ] Keep dataset files and API credentials out of Git unless distribution is authorized; explain how authorized users obtain the data.

## 3. Make training and inference reproducible

- [ ] Document the actual training configuration and command, including the reported 100 epochs if confirmed by logs/configuration.
- [ ] Document inference on images and camera frames, expected input format, and output fields.
- [ ] Document the Raspberry Pi HMI flow and clarify whether it displays class names only or also boxes/confidence values.
- [ ] Provide a small, license-cleared sample or synthetic fixture for tests without committing restricted dataset content.
- [ ] Add tests for preprocessing, class mapping, detection output, and HMI integration where applicable.

## 4. Reproduce and report results

- [ ] Define what the report's approximately 95% accuracy measures and reproduce it on a documented held-out split.
- [ ] Report per-class precision, recall, F1, and appropriate object-detection metrics such as mAP when available.
- [ ] Preserve the confusion matrix and F1 curve from the actual experiment, with provenance and a reproducible command.
- [ ] Reproduce the reported below-100-ms inference time; specify hardware, software, device, model, image size, warm-up, timing boundaries, sample count, and aggregation.
- [ ] Evaluate and document errors for U-turn and railway-crossing signs, plus relevant lighting, weather, viewpoint, blur, occlusion, and sign-condition cases.
- [ ] Do not use randomly sourced web images as a substitute for a documented evaluation split; confirm rights before publishing any examples.

## 5. Release responsibly

- [ ] Review Roboflow dataset terms, upstream YOLOv5 license, dependency licenses, and checkpoint terms.
- [ ] Choose a license for original repository work only after checking incorporated material and permissions.
- [ ] Add real hardware photographs, HMI screenshots, or detection examples only when they are from the project and cleared for publication.
- [ ] State clearly that the system is an academic prototype and is not safety-certified for driving decisions or vehicle control.
- [ ] Add automated tests/CI that do not download restricted data, expose API keys, or require large model weights.

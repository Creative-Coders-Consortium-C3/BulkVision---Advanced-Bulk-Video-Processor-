# BulkVision - Advanced Bulk Video Processor 🎥

A powerful Python-based video processing tool that runs on Google Colab, designed for batch processing videos with features like speed adjustment, watermarking, and various video enhancements. Perfect for content creators, video editors, and social media managers who need to process multiple videos with consistent settings.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1I7l0xPchH-_95GmkyHY7rIfRn-ECTa_r?usp=sharing)

## 🌟 Features

- **Batch Processing**: Process multiple videos simultaneously
- **Video Enhancement**:
  - Speed adjustment
  - Pitch control
  - Brightness, contrast, and saturation adjustment
  - Volume boost
- **Watermark Management**:
  - Custom watermark positioning (top-right, top-left, bottom-right, bottom-left)
  - Adjustable watermark size
  - Optional watermark flipping
- **Video Manipulation**:
  - Video flipping capability
  - Crop functionality
  - High-quality output encoding using NVIDIA GPU acceleration
- **User Interface**:
  - Interactive controls with sliders and checkboxes
  - Real-time progress tracking
  - Detailed logging system

## 📋 Prerequisites

- Google Account (for Google Colab and Drive access)
- NVIDIA GPU support (for optimal processing speed)
- Input videos stored in Google Drive
- Watermark image (PNG format recommended)

## 🚀 Setup Instructions

1. **Open in Google Colab**:
   - Click the "Open in Colab" button above
   - Or use the direct link to the notebook

2. **Mount Google Drive**:
   - The script will automatically prompt you to mount your Google Drive
   - Accept the authorization request

3. **Prepare Your Files**:
   - Create these folders in your Google Drive:
     - `/MyDrive/Uploader Video` (for input videos)
     - `/MyDrive/output folder` (for processed videos)
   - Place your watermark image at `/MyDrive/c3.png`

## 💻 Usage Guide

1. **Configure Processing Settings**:
   - **Speed**: Adjust video playback speed (0.5x to 2.0x)
   - **Pitch**: Modify audio pitch (0.5x to 2.0x)
   - **Video Enhancement**:
     - Brightness (-1.0 to 1.0)
     - Contrast (0.0 to 2.0)
     - Saturation (0.0 to 2.0)
   - **Audio**: Volume boost (-20dB to +20dB)
   - **Watermark Options**:
     - Position selection
     - Flip toggles for video and watermark

2. **Start Processing**:
   - Click the "Process Videos" button
   - Monitor progress through the progress bar
   - Check the log file for detailed processing information

## 📊 Output

- Processed videos are saved with 'processed_' prefix
- Output videos maintain high quality using H.264 NVIDIA encoding
- Original metadata is stripped for privacy
- Detailed logs are generated for troubleshooting

## ⚠️ Limitations

- Requires Google Colab with GPU runtime for optimal performance
- Input videos must be in common formats (mp4, avi, mov, mkv)
- Watermark must be in PNG format
- Processing speed depends on:
  - Video file sizes
  - Selected enhancement options
  - Google Colab's GPU availability

## 🔍 Troubleshooting

Common issues and solutions:

1. **GPU Not Available**:
   - Change runtime type to GPU in Colab
   - Wait for GPU availability if resources are busy

2. **File Not Found Errors**:
   - Verify Google Drive paths
   - Check file permissions
   - Ensure proper Drive mounting

3. **Processing Errors**:
   - Check video file format compatibility
   - Verify watermark file existence and format
   - Review log file for specific error messages

## 📝 Logging

The script maintains detailed logs including:
- Processing start and completion times
- FFmpeg command details
- Error messages and warnings
- Processing status for each video

## 🤝 Contributing

Feel free to:
- Report issues
- Suggest improvements
- Submit pull requests

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- FFmpeg for video processing
- Google Colab for GPU support
- NVIDIA for NVENC encoding
- IPython widgets for the UI

Made with ❤️ for the Creative Coders Consortium (C³) community

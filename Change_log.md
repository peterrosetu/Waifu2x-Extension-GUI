# Change log
---
#### [📝中文版 更新日志](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/blob/master/Change_log_CN.md)

#### [💾Latest stable release](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/latest)
---
## v3.127.01
- NEW Model: V2 update for Omni-Small-W2xEX video upscaling model, featuring better detail reconstruction and deblur capability compare to V1.
- NEW Feature: Added [Presets] for [Custom Resolution] to allow for quick and easy resolution adjustment.
- NEW Feature: Added a [View Output Folder] button for quick access to the output directory.
- Improved compatibility with RTX 50 GPUs for users in certain region.
- Fix bug: The video encoder quality setting did not take effect when [Process Video by Segment] was enabled.
---
## v3.126.01
- NEW Frame Interpolation Model: [RIFE-v4.26], higher quality, Enhanced Stability for Drastic Movements.
- NEW Feature: Now you can keep the transparent background of the GIF after frame interpolation by enable [Keep Alpha Channel] at image settings tab.
- NEW Feature: Now GIF also supports [Target FPS] mode of frame interpolation.
- Update settings presets.
- Now waifu2x will automatically correct the FPS of the GIF output to improve compatibility with media players.
- Improve synchronization between the interpolated GIF and the source GIF.
- Improve code related to reading GIF duration to enhance compatibility with edge cases.
---
## v3.125.01
- NEW Feature: GIF Frame Interpolation.
- You can access GIF Frame Interpolation by enable [Frame Interpolation] option at the Home tab.
- You can enable [Optimize Looped GIF] at the [Image settings] tab.
- [Scene Shift Detection] also supports GIF Frame Interpolation, you can enable it at [Video Settings] tab.
---
## v3.124.01
- NEW Model: Omni-Small-W2xEX, an ESRGAN model trained for Video upscaling, featuring better detail reconstruction and enhanced denoising capability compare to Omni-Mini.
- [Override] toggle for [Presets] and [Custom] modes of the [Maintain consistent Video FPS] feature. When enabled, the specified FPS will always take precedence regardless of whether frame interpolation is active.
- Auto model selection for Video upscaling when using ESRGAN engine.
- Add a button for quickly adjusting the RAM drive size, which will be set to 85% of the available RAM.
- Add right-click menus for [Video Color Management], making it easier to switch between commonly used values.
- Update documentation.
- Update settings presets.
- Fix bug: RTX 50 series card might stuck at compatibility test.
---
## v3.123.01
- NEW Model: V2 Update for Universal-Fast-W2xEX ESRGAN model, featuring better detail reconstruction, improved anime upscaling, and enhanced denoising capability.
- Enhanced Video Color Fidelity: further improve the color accuracy of the default JPEG frame codec while still remaining fast and space-efficient.
- Improvements and bug fixes for [Maintain consistent Video FPS].
- Show a notification about slow processing speed when the highest quality presets are selected.
- Updated documentation for Universal-FastV2-W2xEX.
- Fixed bug: When using Vulkan engines with multiple GPUs, disabling the CPU (-1) could cause issues.
- Fixed bug: Incorrect status when loading a [Files List] file.
- Code optimization.
- Fix UI issues.
- Other bug fixes.
---
## v3.122.01
- New Feature: Better FPS Control for Rendered Video, add [Presets] and [Custom] modes for [Maintain consistent Video FPS].
- New Feature: Added support for 10-bit color depth settings in video encoder settings, improved video quality and more efficient video compression.
- Fix bug: [Maintain consistent Video FPS] doesn't work when [Process video by segment] is enabled.
- Fix bug: [Maintain consistent Video FPS] doesn't work when using RTX Super-res.
- Fix bug: In some situations, video frame interpolation doesn't work when using RTX Super-res.
- Fix bug: In some situations, the cache files are not automatically deleted after finished processing when using RTX Super-res.
---
## v3.121.01
- New RIFE frame interpolation model: [v4.22-lite], provides higher quality than the previous models.
- Add introduction document for Real-ESRGAN models.
- Add a [Select folder] button for [Output Folder].
- When switching the "Image Style" of the ESRGAN engine, the model's image style label in the engine settings tab will be highlighted.
- Add a [Help] button for [Import ESRGAN models] settings.
---
## v3.120.01
- NEW ESRGAN Model: [Photo-Small-W2xEX], fast photo upscaling model, achieved higher photo upscaling quality compared to [Universal-Fast-W2xEX] while maintained similar speed.
- NEW Feature: AV1 Video Encoder support.
- Add SVT-AV1 software encoder.
- Add Nvidia, Intel, and AMD AV1 hardware encoder.
- Update settings preset to utilize the new model.
- Better compatibility with AV1 video codec.
- Update RIFE engine.
- Update GIF plugin.
- Update other plugin.
---
## v3.119.01
- NEW Feature: Better GIF quality, GIF now supports [Transparent image Clarity Enhancement].
- V2 update for Omni-Mini Real-ESRGAN model, improving its image quality without compromising performance.
- Improve the compatibility of [Video Color Management].
---
## v3.118.01
- New RIFE model: [v4.17-lite], compared to the previous Lite model, it can generate more stable frames.
- Additional options for quick Image resize and compress:
- [Do not upscale]: If images resolution is lower then the Custom resolution, they will only be converted(compressed).
- [Ignore scale ratio]: Always ignore scale ratio settings when using [Convert format ONLY (Static Images)].
- [Skip if not smaller]: Converted image will be deleted if its file size is not smaller than the original. The original image will be copied to output folder instead.
- [Skip low resolution images]: When [Convert format ONLY (Static Images)] and [Resize] is enabled, only process images when their resolution is higher then Custom resolution.
- Fix bug: [keep aspect ratio by expanding] not working properly when upscaling images.
---
## v3.117.01
#### Change log:
- New Real-ESRGAN model: [Omni-Mini-W2xEX], a super fast tiny model designed to mimic the quality and speed of RTX Super-resolution, bring RTX Super-res capability to ALL platforms.
- Upgrade Real-ESRGAN [Sequential decoding] to [Image decode threads]. Boost image upscaling performance by auto adjust decode threads based on PCs hardware, up to 87.94% faster during testing.
- Fix bug: In some situations, number of frames does not meet expectation after frame interpolation.
---
## v3.116.01
#### Change log:
- New RIFE model: [rife-v4.15-lite], compared to the previous Lite model, it offers higher quality, faster speed, and reduced VRAM usage.
- New feature: Added a [Resize] option for [Convert format ONLY(Static Image)], using fast scaling algorithm (not super-resolution), capable of instant and simultaneously scaling, compressing, and converting image formats.
- Updated automatic thread allocation algorithm for RIFE frame interpolation engine, improving stability.
- Added a [Reset] right-click menu option for [Static Image Quality], facilitating quick resetting of quality values to 100.
- Optimized code performance.
- Improved UI.
- Fixed issue: [Transparent image Clarity Enhancement] may cause dark parts of some images to become semi-transparent.
- Fixed potential UI option conflicts.
- Removed some historical legacy UI errors.
---
## v3.115.01
#### Change log:
- NEW [Photo-HQ-W4xEX] Real-ESRGAN model, a high-quality photo upscale model. Compared to previous models, it better preserves details and generates cleaner images.
- New Feature: [Automatic Video Deinterlacing], automatically detect interlaced videos and perform deinterlacing before upscaling (frame interpolation).
- Optimize UI performance
- Improved compatibility with some regional formats.
---
## v3.114.01
#### Change log:
- NEW RIFE frame interpolation model: [RIFE V4.17], which has higher quality and can generate more stable frames compared to the previous v4.14 model.
- Significantly faster video encoding speed: When [Process video by segment] is enabled, a new method will be used to assemble video segments, reducing the time spent assembling segments from minutes to seconds in tests.
- Improved the [Video Color Management] UI to support direct selection of all pixel formats supported by the current video encoder.
- Switch default video container format to MKV.
- Optimized UI performance.
- Fixed an issue when [Process video by segment] is enabled, frame interpolation might cause the video stream and audio stream to be out of sync.
- Fixed an issue where a small part of the content might be omitted at the end of the video when [Process video by segment] is enabled.
- Fixed an issue where using [Optimize Looped video] might generate extra duplicate frames, resulting in unsmooth loop playback.
- Fixed an issue where extra frames appeared at the end of the video after frame interpolation.
- Fixed an issue where enabling both [Target FPS] and [Optimize Looped video] could cause errors.
- Fixed an issue where using [Target FPS] to interpolate very short videos resulted in an actual frame rate lower than expected.
- Fixed a conflict issue between [Speed Boost] and [Optimize Looped video].
- Fixed a conflict issue between [Scene Shift Detection] and optimized looped videos.
- Fixed compatibility issues with the latest version of ffmpeg and updated the built-in ffmpeg to the latest version, preparing for future support of more video encoders and decoders.
- Fixed compatibility issues with the latest version of ffprobe and updated the built-in ffprobe to the latest version.
- Fixed a rare issue where Real-ESRGAN might freeze when processing videos and animated images.
- Updated the User Guide, adding jump links to the directory.
- Updated daily tips.
- Corrected typos.
---
## v3.113.01
#### Change log:
- NEW UI Design for [Video Encoder] settings.
- NEW Feature: ProRes video decoding & encoding. (Location: Video settings tab, Video Encoder)
- NEW Feature: [Sequential decoding] for Real-ESRGAN, reduce CPU usage during image decoding and increase performance.
- Performance optimization for [Anime-HQ-W4xEX] Real-ESRGAN model.
- Better multi-threaded performance when upscaling images using Real-ESRGAN.
- [Encoding Quality] and [Hardware-accelerated encoding] are now merged with the new [Video Encoder] settings.
- Fix bug: Some PCs will stuck at image decoding for a long time when using RealESRGAN to upscale static images.
---
## v3.112.01
#### Change log:
- NEW [Anime-HQ-W4xEX] Real-ESRGAN model for High Quality Anime upscaling, which retains detail better and can generate cleaner image compare to previous models.
- NEW Feature: [Video Color Management], software now can automatically adjust color-related parameters to achieve better color accuracy, or you can adjust these parameters by yourself. (Location: Video settings tab)
- Updated [Auto optimize engine settings] to boost the performance of Real-ESRGAN, up to 48% faster than the previous version.
- Better RIFE Auto model selection, now you can tell Waifu2x to use v4.14 model instead of v4.13-lite when automatically selecting model.
- Some UI improvements.
---
## v3.111.01
#### Change log:
- NEW [RIFE-v4.14] model for Higher quality video frame interpolation, which could generate more stable results compare to previous models.
- NEW [RIFE-v4.13-lite] model for Fast and High quality frame interpolation, which is 30% faster than 4.14 model but could achieve similar quality.
- NEW [Auto-Select] feature, automatically select rife model based on your PCs hardware and resolution of the video. (Enabled by default)
- Built-in [User guide] to help new users quickly get started with the software. (Location: Home tab, big question mark icon in the lower right corner)
- [Universal-Fast-W2xEX] RealESRGAN Model is now up to 30% faster by updating [Auto optimize engine settings].
- Update [Settings presets] to utilize the new [Universal-Fast-W2xEX] RealESRGAN Model.
- Fix some UI issues.
- Fix bug: Pausing while processing frame folders may cause the software to crash.
---
## v3.110.01
#### Change log:
- NEW [Universal-Fast-W2xEX] Model for RealESRGAN engine, designed for fast photo upscaling, 30.5x faster than the RealESRGAN-x4plus model while retain decent image quality.
- NEW Feature: Now you can select [Preset] for Nvidia and Intel hardware encoders, which will affect the quality of the result video. (Location: Video settings, Hardware-accelerated Encoding)
- NEW Feature: [Stop then excute action], Stop right after the currently "Processing" files are finished, then execute an action. (Location: Home tab, in the "Do nothing(when finished)" options list)
- Add [Copy] and [Paste] buttons for the right-click menu of [Output path folder].
- Update several plugins.
- Some UI improvements
- [Optimize Looped video] setting will be saved like other settings.
- Fix bug: In certain situations, NCNN-Vulkan engines will randomly get stuck.
---
## v3.109.01
#### Change log:
- NEW Feature: [Encoding Quality], adjust video encoding quality when using software and hardware encoders. (location: video settings tab)
- NEW Feature: [Stop process new files], automatically stop after finished processing current tasks. (Location: Home tab, in the "Do nothing(when finished)" options list)
- When output upscaled images, replace [_Compressed] with [_Q<Static Images Quality value>], like [_Q95], when [Static Images Quality] taken effect.
- NEW video subtitle processing method, better video compatibility.
- Automatically disable Dynamic RAM Cache after the RAM Disk is detached.
- Fix bug: When there are multiple subtitles in one video, the output video might be broken.
---
## v3.108.01
#### Change log:
- NEW Feature: [Import frames folder], browse and add folders of Frames Images for frame interpolation.
- NEW Feature: [Reduce Video FPS], reduce frame rate of the Video before frame interpolation and upscaling. (Additional settings tab, Tools section)
- NEW Feature: [Copy Skipped files], when enabled, also Copy Skipped files to the output folder. (Home tab, output folder section)
- NEW Feature: Now you can adjust how many threads [Convert format ONLY (Static Images)] will use by adjusting: [Engine settings, Number of threads (Super-resolution), Image].
- Significantly improved UI performance, now the Files list UI can handle large amount of files much better than before.
- Optimize code related to video processing.
- Add m4v to the default video file extensions list.
- Fix bug: Real-CUGAN might output incorrect color in certain situations.
- Fix several bugs related to [Convert format ONLY (Static Images)].
- NEW Feature: [Frame interpolation for frames folder] now supports [Delete original files], [Replace original fils] and [Output folder]
- Fix bug: When using [Frame interpolation for frames folder], some original frames might be incorrectly deleted after frame interpolation.
---
## v3.107.01
#### Change log:
- NEW Feature: [Speed Boost 2.0], HUGE Speed boost for duplicated frames detection, faster & more accurate, which means [Speed Boost 2.0] can save way more time then previous version.
- NEW Feature: More [Save as] formats for animated webp: apng, mp4 and webm.
- NEW Feature: [Sync video aspect ratio], Synchronize sample aspect ratio with display aspect ratio.
- Add warning pop-up for [Delete original files] and [Replace original file] options.
- Improve image quality of APNG and WebP upscaling.
- Improve UI, and fix incorrect description.
- Complete translation.
- Fix bug: Broken output when using some engines to upscale WebP and APNG.
- Fix bug: When running on PCs with new(high-end) CPUs, occasionally waifu2x will stuck during frame interpolation.
- Fix bug: When frame interpolation and RTX Super-res both enabled, Video sampling might stop working.
---
## v3.106.01
#### Change log:
- NEW Feature: [Scene Shift Detection 2.0], HUGE Speed boost for Scene Shift Detection, 65x faster than the previous version, which means Scene Shift Detection won't cost any extra time during frame interpolation.
- NEW Feature: [Gif & APNG] option, when enabled, the Animated WebP quality value will also be used when saving APNG and GIF as WebP. (location: Image settings tab)
- NEW Feature: Add [Sync with Home] option for Animated WebP, when enabled, the quality value of Animated WebP will be synced with [static images quality] value at the Home tab. (location: Image settings tab, enabled by default)
- Improved video quality, especially when using hardware encoders.
- When [Gif & APNG] option of Animated WebP is enabled, gif and apng will automatically be saved as WebP.
- Fix bug: In some situations, [Speed boost] could not restore frames and will result in failure.
- Fix bug: In some situations, the [put PC to sleep after finished] feature won't work.
- Fix bug: When [Video sampling] enabled, RTX Super-resolution engine might unable to upscale the video.
- Fix bug: Click the "Execute NOW" button of finish action might crash the software.
- Fix bug: In some rare situations, might unable to encode the final video when process video by segment is enabled.
---
## v3.105.01
#### Change log:
- NEW Feature: Animated WebP support, ALL super-res engines can now upscale Animated WebP images.
- NEW Feature: Now you can save Animated WebP as GIF. (location: Image settings tab)
- NEW Feature: Now you can adjust the quality of upscaled Animated WebP. (location: Image settings tab)
- Variable frame rate support for Animated WebP, other animated pics formats will also support this in the future updates.
- Improved launcher, more issue detection and better pop-up message.
- Fix bug: Always failed to upscale APNGs when their suffix are in upper cases.
- Fix bug: When loading settings preset files from older version, some options will be reseted.
- Fix bug: Messages may contain errors when processing Animated WebP.
---
## v3.104.01
#### Change log:
- NEW Feature: [Auto archive Files List]: Automatically saves Files List every 15 seconds after starting to process files.(Location: Additional settings tab, enabled by default)
- NEW Feature: [Skip Failed files]: Always skip "Failed" files in the files list.(Location: Additional settings tab, disabled by default)
- Improved [Auto Engine optimization] for Real-ESRGAN engine, better picture upscaling performance on most PCs.
- Code optimization, imporve UI performance.
- Add some necessary messages for Save(Read) settings presets.
- Fix bug: The [Priority] setting of RTX Super-resolution engine was not working.
- Fix bug: Always re-process finished files.
- Fix bug: Thread blocking when using Real-ESRGAN engine with auto adjusted settings.
- Fix bug: UI shrinks after loading settings preset file.
- Update ImageMagick.
- Better tooltips.
---
## v3.103.01
#### Change log:
- NEW Feature: [Save & Read settings presets files], Now you can save(and read) your settings as custom preset files.
- NEW Feature: [Transparent image Clarity Enhancement] now supports multi-threading, significantly improves efficiency.
- NEW Feature: Add a right click menu for the [Limiter] of [scene shift detection], now user can select how many threads will be running during [scene shift detection].
- NEW Feature: Now software will automatically check the integrity of current installation, and will display a warning when files are missing.
- Move the [Prioritize Image Quality] option of RTX Super-resolution to Home tab for easy access.
- Upscaling APNG while enabled [Transparent image Clarity Enhancement] is now faster, up to 50% faster compare to the last version.
- Faster APNG upscaling when using SRMD-CUDA and RTX Super-resolution.
- Improve UI performance.
- Add necessary status messages for [Transparent image Clarity Enhancement] to avoid confusion.
- Other performance optimization.
- Update ImageMagick.
---
## v3.102.01
#### Change log:
- NEW feature: RTX Super-resolution engine now supports APNG upscaling.
- NEW Feature: ALL super-res engines now supports [Transparent image Clarity Enhancement] when upscaling APNG.
- Improve SRMD-CUDAs compatibility with media that has alpha channel.
- Improve SRMD-CUDAs compatibility with APNG.
- Performance optimization.
- Fix bug: UI error when using [Quick engine switch].
- Fix bug: Progress display error when using some engines to upscale APNGs.
- Complete translation.
---
## v3.101.01
#### Change log:
- New Feature: [Prioritize image quality] option for RTX Super resolution, improve image quality in most situations, especially when upscaling low resolution media.
- New Feature: [Settings Presets] now supports RTX Super resolution engine.
- Add [Always disable denoise] option for RTX Super resolution.
- Improved device compatibility of RTX Super resolution.
- Performance optimization.
- Update ImageMagick.
- Fix bug: Might unable to upscale video when using RTX Super resolution and HEVC encoding at the same time.
- Fix bug: Auto-retry is not working when using RTX Super resolution to upscale videos.
- Fix typo in the tooltips.
---
## v3.100.01
#### Change log:
- Significantly improved [Files List] UI performance, up to 35x faster files loading speed in the test(16K media files in 800 folders)
- Improved code efficiency related to video, gif and apng processing.
- Code optimization, improved UI and scheduler performance.
- Improved video quality when using Nvidia video encoder
- Better video compatibility when using RTX Super-res.
- Improve mp4 conversion to avoid potential compatibility issue.
- Improved audio quality when encoding mp4 video.
- Improve stability of RTX Super Resolution engine.
- Simplified video compatibility checker.
- Add a "help" button next to the RTX Super-res on the compatibility test page.
- The result of the compatibility test button at the engine settings of RTX Super-res is now connected to the [Compatibility test] tab.
- Fix bug: Unable to upscale some videos when using RTX Super Resolution.
- Fix bug: Audio and video might out of sync when using RTX Super Resolution to upscale some videos.
- Fix bug: When using RTX Super Resolution, might unable to upscale video when frame interpolation is enabled.
- Fix bug: Unable to detect and fix some video compatibility issue of RTX Super Resolution.
- Fix bug: In some rare occasions, unable to detect duplicated files when loading files to [Files List].
---
## v3.99.01
#### Change log:
- NEW Super-resolution Engine: RTX Super Resolution, a fast and light-weight upscaler designed for Nvidia RTX GPUs.
- Exclusive enhancements for RTX Super Resolution like Alpha channel support, various input/output formats and more.
- New Feature: [Auto Apply] option for Custom resolution: When adding new files, the current [Custom resolution] setting will be automatically applied to ALL files.
- When upscaling and interpolating videos, videos with frame rate higher than the specified frame rate are no longer simply skipped, but only upscaled.
- Update FFmpeg
- Update ImageMagick
- Fix bug: Real-ESRGAN can not upscale media correctly when 2d and 3d models are different.
- Fix bug: When using certain settings, unable to encode video after upscale and frame interpolation.
- Fix bug: Incomplete closing process.
- Fix typo.
---
## v3.98.01
#### Change log:
- NEW model for Real-ESRGAN engine: Photo-Conservative-x4
- NEW Feature: [Pause after decoding] option, automatically pause after finished decoding the video, until the user clicks the [Continue] button. (Additional settings, disabled by default)
- NEW Feature: Split the models list of Real-ESRGAN to 2 lists, [3D Real-life] and [2D Anime] for easier use.
- Smarter [Limiter] for Scene Shift Detection, automatically adjusts the load according to the progress.
- Optimize scene shift detection scheduler.
- Improve GUI.
- Improve the stability of [Limiter] for Scene Shift Detection.
- Update ImageMagick.
- Update ffmpeg.
- Code optimization.
- Fix bug: [Always pre-process images with Alpha Channel] not working properly when processing images with invalid alpha channel.
- Fix bug: Some warning messages are outdated and incorrect.
- Fix bug: [Keep Aspect Ratio By Expanding] not working as intended.
---
## v3.97.01
#### Change log:
- ★ NEW Real-ESRGAN models: RealESR-General-x4v3 and RealESR-General-WDN-x4v3
- ★ NEW Feature: [Same as original image] option, save image as the same format of the original image.(only static images)
- ★ NEW Feature: [Reserved VRAM], reserve part of VRAM to improve stability, you can adjust it at [Additional settings] tab.
- NEW Feature: Add [Reset to default] buttons for Input file extensions.
- NEW Feature: Now you can disable [Constant Rate Factor (CRF)] in the Custom video settings.
- Improved Real-ESRGAN auto settings optimization.
- Improve UI and default settings.
- Code optimization.
- Update ImageMagick.
- Update ffmpeg.
- Fix bug: [Bitrate(video)] setting in the [Custom video settings] often will not take effect.
- Fix bug: Unable to save images to PNG when using [Convert format ONLY (Static Images)].
- Fix bug: Some output images will be broken when using [pro] models of Real-CUGAN.
- Fix bug: UI issues related to Real-ESRGAN engine.
---
## v3.96.01
#### Change log:
- New RIFE-v4.6 model, better frame interpolation quality.
- New feature: [Auto-Create output folders], automatically create output folder when needed, including all parent folders.
- New feature: Now RIFE v4 and v4.6 models supports TTA.
- Better auto engine settings optimization algorithm.
- Auto engine settings optimization now supports all Real-Cugan models.
- Improve UI.
- Update Rife-ncnn-vulkan.
- Update ImageMagick.
- Update ffmpeg.
- Fix bug: Switch Real-Cugan models won't work properly when processing videos and GIFs.
---
## v3.95.23
#### Change log:
- NEW Feature: New aspect ratio strategy: [Specify Minimum resolution]
- Performance optimization.
- Better error report and tooltip.
- Fix bug: When processing static images, upscale ratio with decimal digits may not work properly.
- Fix bug: When processing static images, 1x scale ratio isn't working when using some engines.
- Fix bug: When processing static images, [Specify Width(Height) ONLY & Keep Aspect Ratio] not working properly.
- Fix translation error.
- Update heif plugins.
- Update ImageMagick.
- Update ffmpeg.
---
## v3.95.01
#### Change log:
- NEW Feature: Display current progress when Finding scene shifts.
- Newly redesigned internal image resizer, better compatibility and image quality.
- Improved image quality.
- Improved compatibility.
- Performance optimization.
- Reconstruct some codes to improve stability.
- Update FFmpeg
- Update ImageMagick
- Remove some unnecessary warning messages.
- Fix bug: In certain situations, failed to output final image when using Real-ESRGAN and [Transparent image Clarity Enhancement] at the same time.
- Fix bug: In some situations, the final image is incompatible with some image viewers.
- Fix bug: [Automatic file list scrolling] was not working.
- Fix bug: UI logical error.
- Fix bug: Unable to reach target frame rate after video frame interpolation.
---
## v3.94.01
#### Change log:
- NEW feature: Now [Scene Shift Detection] can running in parallel with video frame interpolation, will significantly improve performance and efficiency.
- NEW feature: Add [Quick Engine Switch]. at [Home] tab for easy super-res engine switching.
- NEW feature: ALL 6 IFRNet models now supports "Auto-Adjust" multithreading.
- NEW feature: ALL 10 RIFE models now supports "Auto-Adjust" multithreading.
- NEW feature: Thread [Limiter] option for [Scene Shift Detection], can improve PC responsivity during during [Scene Shift Detection].
- Improve code efficiency and stability.
- Update FFmpeg and ImageMagick
- Bug fix.
---
## v3.93.01
#### Change log:
- NEW frame interpolation engine: IFRNet-ncnn-vulkan.
- Add new "Pro" models for Real-CUGAN.
- Faster Real-CUGAN super-resolution.
- Update multiple Engines, reduce overall VRAM usage.
- Real-CUGAN now supports model switching.
- Update auto engine settings optimization strategy.
- More accurate detection method for variable frame rate video.
- Improve compatibility with variable frame rate video.
- Improve user interface.
- Update ALL frame interpolation engines.
- Update Real-CUGAN, RealSR, SRMD(vulkan), Waifu2x(vulkan).
- Fix multiple bugs, fix translation error.
---
## v3.92.01
#### Change log:
- NEW Feature: [Transparent image Clarity Enhancement]. Improve clarity when upscaling images with transparent background(Alpha channel).
- ALL engines supports [Transparent image Clarity Enhancement] when processing Static Images and PSD.
- NEW Feature: After the compatibility test, automatically switch to compatible engines for new users.
- Improve Auto-optimize Engine settings.
- Improve UI performance.
- Fix bug: Unexpected frame rate change of the result video.
- Other bug fix and improvements.
---
## v3.91.01
#### Change log:
- New Feature: Import and use 3rd party model for Real-ESRGAN engine.
- New Feature: Bring back lossless PNG compression for static images.
- New Feature: Bit depth adjustment and 16 bit image output for Waifu2x-caffe engine.
- New Feature: Now you can adjust the size of status console.
- Improve image quality when using custom resolution.
- Better denoise levels support for Real-CUGAN native 4x upscale.
- Smarter model picking for Real-CUGAN.
- Improved automatic multithreading, better utilize the performance of high-end PCs.
- [Constant Rate Factor (CRF)] in the [Custom video settings] now supports more encoders.
- Improve VFR video detection.
- Some UI improvements.
- Improve network stability for checking new updates and update QR code.
- Update several plugins.
- Fix multiple bugs.
---
## v3.90.01
#### Change log:
- Faster Real-ESRGAN super-resolution, up to 240% faster than previous version.
- Faster Waifu2x super-resolution, up to 320% faster than previous version.(Waifu2x-NCNN-Vulkan)
- New AnimeVideo-v3 model for Real-ESRGAN engine, better and faster anime video upscale.
- New Feature: Save GIF as APNG.
- New Feature: [Auto empty Files List], Automatically empty Files List after finished processing.(Disabled by default, additional settings)
- Improve the auto multi-threading performance of Real-ESRGAN and Waifu2x-NCNN-Vulkan.
- Smarter auto multi-threading for Real-ESRGAN and Waifu2x-NCNN-Vulkan.
- Faster image pre-processing.
- Improve default settings.
- Some internal structural improvements for GUI.
- Fix bug: Unable to assemble PSD files.
- Some other bug fix and improvements.
---
## v3.89.01
#### Change log:
- Faster Real-CUGAN super-resolution, up to 60% faster than previous version
- Faster and more Efficient frame interpolationm when using RIFE.
- New feature: Add new option for Real-CUGAN, [Always use 2x models], could improve image clarity in some situations.
- New feature: Save images as JPEG XL format(.jxl)
- New feature: Now you can adjust image quality when save images as AVIF format
- Smarter auto model selection for Real-CUGAN
- Reduce the VRAM usage of RIFE
- Improve the auto multi-threading performance of RIFE
- Improve auto engine settings optimization.
- Fix multiple BUGs.
---
## v3.88.01
#### Change log:
- NEW Super-Resolution Engine: Real-CUGAN-NCNN-Vulkan, high quality 2D anime upscaler.
- New Feature: New Rife-V4.0 model, Faster frame interpolation and less VRAM usage.
- New Feature: Save images as Jfif and Jpeg.
- New Feature: Add Real-CUGAN model for Waifu2x-Caffe.
- Improve custom resolution mechanism, and performance optimization.
- Improve Video, GIF and APNG compatibility.
- Improve settings presets and UI.
- Fix multiple bugs.
---
## v3.87.01
#### Change log:
- New Feature: Now you can choose the Container format of the video output.(At Video Settings tab)
- New Feature: [Keep subtitles (MKV)]: Include subtitles in the final video output.(At Video Settings tab)
- New Feature:[Convert format ONLY (Static Images)]: Only convert format of the images, no further processing.(Additional settings---Tools)
- New Feature: Automatic chroma adjustment option for HEIF/HEIC images.
- New Feature: [Save CFR MP4 to RAM]: Re-direct CFR Mp4 cache to Dynamic RAM Cache.(Optional,Not enabled by default,Additional settings)
- Improve multi-threading performance.
- Update UI and fix typo.
---
## v3.86.74
#### Change log:
- Happy New Year 2022!
- New Audio processing method, better Compatibility, better Quality and Faster speed.
- Improve Auto engine settings optimization.
- Improve GUI, Update plugins.
- Fix multiple bugs.
---
## v3.86.02
#### Change log:
```
v3.86.02:
- Fix bug: Real-ESRGAN Video & GIF upscale fix
v3.86.01:
- New Feature: Add support for RealESRGANv2-animevideo-xsx2(4) model.
- NEW Feature: Save images as HEIC/HEIF format.
- Faster 2D-Anime Video and GIF upscale speed when using RealESRGAN-NCNN-Vulkan engine.
- Multiple GUI improvements to fully utilize the new RealESRGAN model.
- Enhance the compatibility of RealESRGAN-NCNN-Vulkan engine.
- Improve Performance and Compatibility of GIF processing.
- Fix multiple bugs.
```
---
## v3.85.01
#### Change log:
- NEW Feature: Save APNG as other formats, including gif, mp4, webp and webm. (At Image settings)
- NEW Feature: Support GIF with variable frame rate.
- Introduce [Auto I/O redirection] to greatly improve compatibility.(Enabled by default, Additional settings)
- New way to Save and Read GIF, Faster and Better image quality.
- Improve the [Save as other formats] function of GIF, better device compatibility and performance.
- Improve UI.
- Update several plugins, remove useless plugins.
- Fix multiple bugs.
---
## v3.84.01
#### Change log:
- New Feature: Save GIF as other formats, including mp4, webp and webm. (At Image settings)
- New Feature: [Optimize Looped video] option, improve the effcet of frame interpolation.when processing looped video.(At Additional settings)
- Significantly improved the speed and space usage of [Pre-processing Boost].
- Improve video quality, smarter video quality control.
- New hardware decoders: OpenCL and Vulkan.
- New aspect ratio strategy: Specify Width(or Height) ONLY.
- Update FFmpeg and improve compatibility.
- Fix multiple bugs.
- Improve UI, compatibility test and daily tips.
---
## v3.83.21
#### Change log:
- NEW Feature: Save images as PSD.
- Speed up the program startup speed.
- Improve user experience.
- More automation, improve default settings.
- Improve video quality, improve video conversion speed, reduce space usage.
- Update FFmpeg and ImageMagick.
- Fix bug: In some situations, video stream will become shorter when [Pre-processing Boost] enabled.
- Fix UI issues.
---
## [v3.83.01](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.83.01)
#### Change log:
- NEW Feature: [Pre-processing Boost]: Remove ALL unnecessary duplicate frames in the video before processing. Can improve both the processing speed and effcet of frame interpolation.
- NEW Feature: [Remove dupduplicate frames ONLY (Video)]: ONLY remove all unnecessary dupduplicate frames in the video, no further processing.
- NEW Feature: [Remember window size].
- NEW Feature: [RAM Cache Validity Check] toggle, now you can use RAM Disk created by other software after disable this check.
- NEW Feature: [Auto Scroll] toggle for console.
- NEW Feature: Now GUI will be able to detect if the cache disk is full during frame interpolation and super-resolution.
- Global optimization, improve code efficiency, reduce GUI's CPU usage.
- Improve thread scheduling.
- Improve video quality, especially when using hardware encoder.
- Improve MP4 conversion.
- Update FFmpeg, ImageMagick.
- Many other improvements.
- Fix multiple bugs.
---
## [v3.81.01](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.81.01)
#### Change log:
- 🌟NEW Super-Resolution Engine: RealESRGAN-NCNN-Vulkan.
- 🌟Significantly improved the UI performance, especially the Files List UI.
- 🌟NEW Feature: [Video sampling]: Only process part of the video from the start to the end of the time you set.(At [Additional settings] tab)
- Improve internet connection speed.
- Add more settings presets
- Driver version detection for NVENC encoder.
- Improve MP4 conversion.
- Improve pop-up messages.
- And many other improvements.
- Fix multiple bugs.
---
## [v3.73.14](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.73.14)
#### Change log:
- New method for cut video, significantly reduced the extra time cost of processing video by segment.
- Further improve the [Auto-adjust] for frame interpolation.
- Further improve the [Optimize Settings] for super-res engines.
- Reduce the time and resource cost when processing video with certain FPS values.
- Faster Internet connection speed.
- Fix several bugs.
---
## [v3.72.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.72.13)
#### Change log:
- NEW Feature: Upgrade [Auto-reduce] to [Auto-Adjust], now GUI can automatically adjust the number of threads for frame interpolation engine based the source video and PCs hardware.
- All non-natively supported image formats will be pre-processed before being scaled.
- AVIF and HEIC images support.
- Improve [Optimize Settings] for super-resolution engine.
- Fix bug: frame rate of the result gif is wrong.
- Fix bug: Sometimes unable to open local html.
---
## [v3.71.01](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.71.01)
#### Change log:
- New feature: Add [Optimize Settings] button for helping user adjust engine settings based on PCs hardware,including [Block(Tile) size] and [Number of threads].(At [Engine settings] tab)
- Now you can tell GUI to stop showing you warning when enable Hardware-accelerated Encoding & Decoding.
- Resume progress when video frame cache in the RAM is lost.
- Add [GeForce RTX ON] switch for SRMD-CUDA engine.
- Update FFmpeg, ImageMagick, SRMD-CUDA.
- Show a warning when enable [Speed Boost].
- Fix 10 bugs.
---
## [v3.70.02](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.70.02)
#### Change log:
- NEW Feature: [Dynamic RAM Cache]: Now GUI can save & read video caches(frames) from the RAM, which is a lot faster and will protect the lifespan of your hard drive.
- NEW Feature: [Target FPS]: Now you can specify the FPS of the result video(e.g. 120FPS).
- NEW Feature: [Hardware-accelerated Decoding]: Now GUI can use GPU to accelerate video decoding.
- NEW Feature: [Frame codec]: Now you can switch the codec of video frames to JPEG to reduce cache size.
- NEW Feature: Now you can adjust the settings of GIF & APNG optimization, they are on the [Image settings] tab.
- NEW Feature: PSD(Photoshop Document) support.
- Improve GUI, Update Anime4K, and fix multiple bugs.
- Fix bug: Unable to display frame interpolation progress correctly when [Multiple of FPS] is higher than [2].
- Fix bug: All EMPTY parent folders will be deleted when delete a folder.
- Fix bug: Unable to update processing progress if the processing speed is extremely fast.
- Fix bug: GUI will becomes laggy when there are too many lines in the Console.
- Fix bug: Sorting the files list by file name does not sort numbers logically.
- Fix bug: Unable to adjust the window size correctly.
---
## [v3.52.11](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.52.11)
#### Change log:
```
v3.52.11:
- Fix typo.
- Fix bug: Unable to detect scene shift correctly when processing Hight-res videos.
- Fix bug: Unable to read images resolution in certain situations.
- Fix bug: "FrameAnalyzeMB" was not deleted in certain situations.

v3.52.10-beta:
- New feature: "Reset [Frame Analysis] Settings" button.
- Improve GUI.
- Improve the default settings of [Frame Analysis].
- Automatically switch to software encoder when hardware encoder unable to convert some videos to CFR MP4.
- More detailed ERROR reports.
- Fix bug: Unable to convert some videos to CFR MP4, caused by hardware encoder.
- Fix bug: Unable to detect failures correctly when processing videos.
- Fix bug: Pixel format parameter was ignored.
```
---
## [v3.52.01](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.52.01)
#### Change log:
```
v3.52.01:
- New Feature: [Keep ALL parent folders]: Keep ALL the parent folders of the source file when output the result file to the output folder.
- New Feature: Now you can change the extension(format) of the result video.
- New Feature: Now you can choose which video Encoder to use when converting video to CFR MP4.
- New Feature: [Hardware-accelerated Encoding]: Using GPU to accelerate video encoding.
- New Feature: [Hyper-threading (SMT)] switch.
- optimize multi-threading performance.
- New Feature: Show available GPUs name when detecting GPU IDs for NCNN-Vulkan engines.
- New Feature: New right-click menu option for [Settings Presets]:[Re-Apply Current Preset]
- Show how many duplicate frames and scene shifts has been found.
- Optimize the performance of [Speed Boost]&[Scene Shift Detection]
- Better High DPI screen support.
- Fix bug: compatibility test stuck at SRMD-CUDA.
- Fix bug: even though PC passed DAIN-NCNN-Vulkan compatibility test, program will still tell the user that all frame interpolation engines are incompatible.
- Fix bug: Unable to generate video when video stream is not the 0 stream.
- Fix bug: Unable to assemble video when [Process video by segment]&[Custom video settings] are both enabled.

v3.51.01-BETA:
- New Feature: [Speed Boost]: Boost video processing speed by analyzing frames.
- New Feature: [Scene Shift Detection]: Detect Scene Shift in the Video to improve the result of video frame interpolation.
- New Feature: [Settings Presets]: Several settings presets provided by the developer.
- New Feature: [Constant Rate Factor(CRF)] adjustment.
- New Feature: [Daily Tip].
- New RIFE-ncnn-Vulkan Model: rife-v3.0,rife-v3.1
- Improve Video quality, Default settings, GUI and scale performance of Waifu2x-NCNN-Vulkan.
- Update rife-ncnn-vulkan, Waifu2x-NCNN-Vulkan.
- Fix bug: Unable to reset all custom video settings.
```
---
## [v3.42.11](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.42.11)
#### Change log:
- Faster APNG processing.
- New Faster methods for resize,assemble and optimize APNG.
- Support for Videos with Multiple Audio Tracks.
- Individual toggle for APNG optimization: [Optimize Gif&APNG].
---
## [v3.41.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.41.13)
#### Change log:
```
v3.41.13:
- New Feature: Automatically try to create output folder when the output folder does not exist.
- New option for system tray menu.
- Compatibility test for APNG plugins.
- Chinese translation.
- Fix bug: Unable to assemble APNG when there are "%" in the path.
- Fix bug: Wrong message were displayed when all files lists are cleared.

v3.41.01-beta:
- New Feature: APNG(Animated PNG) support.
- Improve GUI.
- Some other improvements.

v3.31.21-beta:
- Performance optimization.
- Update FFmpeg, ImageMagick.
- Some other improvements.
```
---
## [v3.31.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.31.13)
#### Change log:
- NEW Super-Resolution Engine: SRMD-CUDA (By @MrZihan).
- Some improvements.
- Fix bug: Frame rate of the result GIF is always 10fps.
---
## [v3.22.26](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.22.26)
#### Change log:
```
v3.22.26:
- New option for system tray menu.
- Fix bug: Unable to naming images correctly when using Anime4k.
- Fix bug: False error report.
- Fix bug: Unable to continue process existing video cache when frame interpolation is enabled.

v3.22.25-beta:
- Optimize performance.
- Improve description.
- Improve stability.
- Fix bug: Unable to continue process existing video cache when frame interpolation is enabled.

v3.22.24-beta:
- Improve quality of the result video.
- Improve the naming of result files when using Anime4k engine.
- Optimize performance.
- Remove first time start tips.
- Fix bug: Denoise level is still being loaded even though HDN is not enabled.
- Fix bug: Crash when unable to read video or gif info correctly.
- Fix bug: Unstable Internet connection might cause some unexpected error.

v3.22.23-beta:
- Improve quality of the result video.
- Improve the naming of result image.
- Optimize performance.
- Online update for Top Supporters List.
- Redesign the credits page for Top Supporters(patreon).
- Improve description.

v3.22.22-beta:
- New feature: Now you can choose to automatically open the output folder after processing all files by enabling [Auto-open after finished].
- Update FFmpeg&FFprobe, ImageMagick.
- New option for system tray menu.
- Credits page for Top Supporters(patreon).
- Display a notification when program is closing.

v3.22.21-beta:
- New option: [Ignore frame rate mode]
- Improve the progress display of video frame interpolation.
- Fix bug: Sometimes the remaining time cannot be calculated correctly.
```
---
## [v3.22.14](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.22.14)
#### Change log:
```
v3.22.14:
- Improve GUI.
- Complete Chinese translation.
- Fix bug: Might stuck at Waifu2x-Caffe(cuDNN) during the compatibility test.

v3.22.03-beta:
- Add a Patreon button. https://www.patreon.com/aaronfeng
- Optimize performance.
- Fix bug: Video will be skipped even though [Frame Interpolation only(Video)] is enabled.

v3.22.02-beta:
- Optimize performance.
- More detailed tool tips.
- Update FFmpeg&FFprobe.

v3.22.01-beta:
- New Feature: Non-integer scale ratio support.
```
---
## [v3.21.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.21.13)
#### Change log:
```
v3.21.13:
- Complete multi-language translation.
- Fix bug: Turn off screen button doesn't work.
- Fix bug: compatibility test progress bar not working normally.

v3.21.02-beta:
- New Feature: [Multiple of FPS] adjustment is now available for all video frame interpolation engines.
- Improve GUI.
- Fix bug: Potential video cache conflict.
- Fix bug: Unable to generate a video when multiple of fps is higher then 2.

v3.21.01-beta:
- New Frame Interpolation engine: DAIN-NCNN-Vulkan.
- New Feature: Multiple of frames.(Only available when using DAIN-NCNN-Vulkan.)
- Improve GUI.
- Fix bug: Unable to generate a video when frame interpolation failed.

v3.11.33-beta:
- New Feature: Now you can choose when you wanna interpolate the frames, before or after upscaled the frames.(Thanks to @CAFUCSteven for suggestion)
- New options: [Start], [Pause] and [Donate] for system tray menu.
- Add icons for system tray menu.
- Fix bug: The [Background mode] in system tray menu didn't work when frame interpolation is enabled.
- Fix bug: Video cache will be abandoned when frame interpolation setting is changed, even though [Process video by segment] is disabled.
- Fix bug: False error report when pause.

v3.11.32-beta:
- New options: [About] and [Send feedback] for system tray menu.
- Better naming for cache files.
- Optimize performance.
- Update FFmpeg&FFprobe,ImageMagick.
- Fix typo.

v3.11.31-beta:
- New Feature: Show summary after processing all files.
- New Feature: Now you can save multiple files lists.
- No longer need to fix the suffix of mp4 files.
- Optimize performance.
- Remove 日本語 translation.
```
---
## [v3.11.27](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.11.27)
#### Change log:
```
v3.11.26-beta:
- New model: rife-v2.4 for rife-ncnn-vulkan.
- Update rife-ncnn-vulkan.

v3.11.25-beta:
- Add a turn off screen button.

v3.11.24-beta:
- Waiting for the main file processing thread to stop instead of force it to stop when user close the program.
- Improve "Pause".

v3.11.23-beta:
- Optimize performance.

v3.11.22-beta:
- Multithreading of frame interpolation engines will not be enabled by default.
- Update FFmpeg&FFprobe.
- Fix bug: When [Process video by segment] is enabled, if the user forcibly closes the program and then restarts the software to continue processing the video, it may cause a cache error.

v3.11.21-beta:
- Update GUI layout.
- Optimize performance.
- Update ImageMagick,FFmpeg&FFprobe.
- Fix bug: Engine settings are pre-loaded even though it's not being used.
- Fix bug: Unable to overwrite files sometime.
- Fix bug: Cannot fix the suffix of mp4 video when reading files.
```
---
## [v3.11.19](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v3.11.19)
#### Change log:
```
v3.11.19:
- Optimize performance.
- Update GUI.
- Fix bug: Cannot interpolate frames of video with "%" in the absolute path.
- Fix bug: [Hide Text Browser] doesn't work properly.

v3.11.08-beta:
- Fix bug: Failure detection for NCNN-Vulkan engines not working normally.
- Fix bug: Extra commands are always loaded when [Process video by segment] is enabled.
- Fix bug: Compatibility test may provide incorrect results.
- Fix bug: Available GPU ID detection for NCNN-Vulkan engines may provide incorrect results.

v3.11.07-beta:
- Update GUI layout.

v3.11.06-beta:
- New Feature: Automatically enable [UHD Mode] when Ultra High Definition input is detected.
- Much more compact gui.
- Optimize performance.
- Fix bug: Extra commands for video are not loaded when [Process video by segment] is enabled.
- Fix bug: [Automatic file list scrolling] not working normally after user rearrange the files list.
- Fix bug: [Verify] button is enabled when [Multi GPU] is disabled.

v3.11.05-beta:
- Fix bug: Unable to use [Process video by segment] when Frame Interpolation is disabled.

v3.11.04-beta:
- Add a shortcut for enable Frame Interpolation in home tab.
- [Verify] button for Frame Interpolation.
- Complete translation.
- Other improvements.

v3.11.03-beta:
- New Feature: Now you can skip the super-resolution, only interpolate video frames by enable [Frame Interpolation only(Video)].
- Add pause support for frame interpolation.
- Add auto adjust for number of threads of frame interpolation.
- Add failure detection for frame interpolation.
- Remove temporary code for debug.
- Fix bug: If frame interpolation failed in the middle of processing video by segment, clip with wrong frame rate gonna be generated.
- Fix bug: Cannot read video configuration correctly.

v3.11.02-beta:
- New Feature: Video frame interpolation using cain-ncnn-vulkan(@nihui).
- Add tool tips.
- Fix bug: Video frame interpolation engines won't work when there are special characters in the installation path.
- Fix bug: Video frame interpolation setting is not saved in the video configuration file.

v3.11.01-beta:
- New Feature: Video frame interpolation using rife-ncnn-vulkan(@nihui).
- Update Waifu2x-NCNN-Vulkan,SRMD-NCNN-Vulkan,RealSR-NCNN-Vulkan.
- Fix bug: Failure detection for NCNN-Vulkan engines doesn't work as intended when processing GIF and Video.
```
---
## [v2.71.22](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.71.22)
#### Change log:
- The maximum number of threads will no longer be limited by the number of CPU logical cores.
- Speed up the assembly of GIF.
- Kill the sub process that is stuck in the background after stopping processing the file.
- Fix bug: Gif scale ratio is wrong when using Anime4k.
- Fix bug: Modifying the duration of the video clip after pausing and then continuing processing will cause the video sequence to be disordered.
- Fix bug: Hotkey for Remove from list is still enabled when processing files.
- Fix bug: [Time remaining] and [ETA] are still bing calculated even though they are not being displayed.
---
## [v2.71.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.71.12)
#### Change log:
- Significantly improve the efficiency, speed and stability of ALL engines when processing Video and GIF.
- The OLD version of waifu2x-ncnn-vulkan engine will no longer support the use of multiple graphics cards to process GIF and video.
- Fix bug: When custom resolution and video settings are enabled and the video stream bit rate is left 0, the video stream bit rate cannot be calculated normally.
- Fix bug: Scale ratio might be incorrect when using srmd-ncnn-vulkan.
- Fix bug: Unable to assemble gif because ImageMagick is not compatible with new AMD GPU driver.
- Update ImageMagick,FFmpeg&FFprobe.
---
## [v2.62.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.62.13)
#### Change log:
- Improve the performance of SRMD-NCNN-Vulkan.
- Fix bug: Incorrect scale ratio when using SRMD-NCNN-Vulkan.
---
## [v2.62.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.62.12)
#### Change log:
- Speed up the processing of video and gif.
- Abandon python extension to improve performance.
- Improve download speed, video processing flow, multithreading performance and other performance improvements.
- More detailed tool tips, fix typo.
- Fix bug: Cannot process variable frame rate video properly.
- Fix bug: After the compatibility test is over, the waifu2x-caffe process will stay in the background.
---
## [v2.61.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.61.13)
#### Change log:
- NEW Feature: Automatically skip file when its resolution is larger than the specified resolution.
- NEW Feature: CUDA support for Anime4k
- Preload engines settings to improve performance,and other performance improvements.
- Update and adapt to the new version of Anime4K.
- Improve the way of reading picture resolution.
- Improve the GUI based on [@Nova-Aurora](https://github.com/Nova-Aurora)'s suggestion.
- Update FFmpeg&FFprobe,ImageMagick.
- English localization fixes(Thanks to [@Nova-Aurora](https://github.com/Nova-Aurora)), and GUI fixes.
- Fix bug: After the user specifies the processor, the [Disable GPU] option of Waifu2x-Converter will not take effect.
- Fix bug: If pause during the image processing, useless files will be generated.
---
## [v2.59.15](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.59.15)
```
v2.59.15:
- Improve GUI.

v2.59.04-beta:
- Images will only be forced to be saved as PNG when the specified file format does not support Alpha channel.
- Add buttons to adjust the block size to the nth power of 2.
- Performance optimization.
- Edit tool tip.
- Other improvements.
- Update ImageMagick,FFmpeg&FFprobe.

v2.59.03-beta:
- Automatically disable [Save Files List] button when files list is empty.
- More compact GUI, and other improvements.
- Edit tool tip and Chinese translation.

v2.59.02-beta:
- NEW Feature: Reset Files List scale.
- NEW Feature: File count for each kind of file.
- New icons.
- Performance optimization.
- Other improvements to the GUI.
- Complete translation.
- Fix bug: [Add Files] button is not disabled when loading Files list.
- Fix bug: Horizontal header data of the Files List will lost after using the right-click menu of [Remove item].

v2.59.01-beta:
- NEW Feature: Now you can hide components easier by drag the handle.
- Improve GUI design.

v2.58.14-beta:
- NEW Feature: Now you can adjust the horizontal width of the file list.
- Move [Move to Recycle Bin] option to Right-click menu of [Delete original files]
- Other improvements to the GUI.
- Notify users GPU ID list is empty when they try to enable Multi-GPU.
- Optimize performance.
```
---
## [v2.58.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.58.13)
#### Change log:
- NEW Feature: CPU support for waifu2x-ncnn-vulkan.
- NEW Feature: Keyboard shortcuts for Files list.
- Notify user when all files in Files list are Finished or Deleted.
- Update Waifu2x-NCNN-Vulkan,ImageMagick,FFmpeg&FFprobe.
- Compatible with future version of NCNN-Vulkan engines.
- More detailed tooltips.
---
## [v2.57.41](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.57.41)
#### Change log:
- ♥Happy New Year in advance, and thank you for your support of this project in 2020.
- The setting value will not be modified when using Force retry.
- The optimized gif will not replace original gif when it's not smaller than the original.
- Update Waifu2x-converter,Anime4K,ImageMagick,FFmpeg&FFprobe.
- Optimize performance, fix typo(Chinese) and some other improvements.
- Fix bug: Gif files will be misplaced if user put "gif" in the input file extensions list.
- Fix bug: Sometimes Files list randomly scrolls horizontally by itself.
---
## [v2.57.31](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.57.31)
#### Change log:
- Update Anime4K,FFmpeg&FFprobe,ImageMagick.
- Improve performance and compatibility.
- Some other minor improvements.
- ✅Fix grammatical,UI and compatibility issues.
- ✅Fix bug: Unable to process gif and video, when there are % in the file path.
- ✅Fix bug: Cannot read the GPUs List of the latest Anime4K.
- ✅Fix bug: When engines randomly crashes for some unknown reasons, the compatibility test will provide incorrect results.
- ✅Fix bug: Image with alpha channel will still be reprocessed even the current engine doesn't support processing alpha channel.
---
## [v2.57.21](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.57.21)
#### Change log:
- New feature: Intelligently detect whether the Alpha channel is lost, and automatically reprocess the picture.
- New feature: [`Always pre-process images with Alpha Channel`].
- Update ImageMagick.
- Improve stability and performance.
- Fix bug: NCNN-Vulkan engines cannot keep the alpha channel of some special png pics.
- Fix typo.
---
## [v2.57.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.57.12)
#### Change log:
- Optimize the file list, greatly improve the speed of reading files.
- Other prformance optimization.
- Update FFmpeg&FFprobe,ImageMagick.
- Fix typo and grammatical issues in the tooltip.(Thanks to @CaptainStabs for feedback)
---
## [v2.56.95](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.95)
#### Change log:
- New feature: Now you can save pictures in multiple formats.(thanks to [@loafylemon](https://github.com/loafylemon) for suggestion)
- Optimize performance.
- Update FFmpeg&FFprobe.
- Remove redundant function, code and comments.
- Fix bug: Audio and video might out of sync because of the wrong frame rate.(thanks to [@CAFUCSteven](https://github.com/CAFUCSteven) for feedback and assistance in testing.)
- And other minor improvements.
---
## [v2.56.82](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.82)
#### Change log:
- New feature: Now you can sort the files in the file list.
- Other improvements to the file list.
- Add more nice icons.
- Update FFmpeg&FFprobe,ImageMagick.
- Improve performance.
- Reduce cache file.
- Add more tooltip.
- Fix multiple bugs.
---
## [v2.56.71](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.71)
#### Change log:
- New feature: The right-click menu of the file list now supports applying and canceling custom resolution setting of individual file.
- New feature: Now you can choose to keep the parent folder when outputting files to the output path.
- Performance optimization.
- Improve user interface.
- Update and adapt Anime4KCPP, FFmpeg&FFprobe, ImageMagick.
- Fix multiple bugs.
---
## [v2.56.52](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.52)
#### Change log:
- New feature: Now you can enable [Replace original file] to directly replace the original file with the processed file. (Additional settings, optional, disabled by default)
- Performance optimization.
- Update FFmpeg&FFprobe, ImageMagick.
- Fix bugs.
---
## [v2.56.46](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.46)
#### Change log:
- Automatically check for updates after switching update channels.
- Add a right-click menu for the [Remove Item] button.
- Improve Files List.
- Performance optimization.
- Update waifu2x-caffe, ImageMagick.
- Enhance the compatibility of waifu2x-caffe engine and Anime4k engine.
- Jump to the homepage after automatically adjusting engine settings.
- Fix bug: the right mouse button cannot select the file in the Files List.
---
## [v2.56.41](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.41)
#### Change log:
- New feature: Add a progress bar for compatibility test.
- Update FFmpeg&FFprobe.
- Fix typo.
- Complete multilingual translation.
- Fix bug.
---
## [v2.56.35](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.35)
#### Change log:
- According to the length of the video, automatically determine whether to enable segmentation processing.
- Update the NCNN-Vulkan series engines.
- Update FFmpeg&FFprobe.
- Fix multiple bugs.
---
## [v2.56.32](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.32)
#### Change log:
- Add more actions (shut down, sleep, hibernate, restart) that can be performed after processing all the files. (Thanks to @Michael18751 for the suggestion)
- Adapt to the new version of FFmpeg.
- Update FFmpeg&FFprobe, ImageMagick.
- Performance optimization.
- Fix multiple bugs.
---
## [v2.56.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.56.12)
#### Change log:
- Anime4k engine can support adjusting the noise reduction level after enabling [HDN mode].
- Add support for automatic detection of Alpha channel for Anime4k engine. (The new version of Anime4k engine supports processing Alpha channel)
- Add right-click menu options for [Files List]: [Open selected file], [Open the folder of the selected file] and [Remove selected file from list]
- Add a right-click menu for [Output Path] to open the output path folder.
- Update FFmpeg & FFprobe, Anime4K.
- Fix multiple bugs.
- Other improvements.
---
## [v2.55.24](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.55.24)
#### Change log:
- Update FFmpeg & FFprobe, Python extension, waifu2x-ncnn-vulkan, ImageMagick.
- Performance optimization.
- Other improvements.
---
## [v2.55.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.55.12)
#### Change log:
- New feature: Add buttons to show the current multi-gpu settings for all engines.
- Update FFmpeg&FFprobe, ImageMagick.
- Performance optimization.
- Improve multi-language support.
- Fix multiple bugs.
---
## [v2.54.13](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.54.13)
#### Change log:
- Update QT to 5.15.0 than recompile the program.
- When it is detected that the custom resolution contains an odd number, the custom resolution will be automatically corrected for the video.
- After enabling [Ban Gitee], automatically detect whether raw.githubusercontent.com can be connected.
- Update waifu2x-ncnn-vulkan, srmd-ncnn-vulkan, realsr-ncnn-vulkan, FFmpeg & FFprobe.
- Performance optimization.
- Fix multiple bugs.
- [And many other improvements, click to view detailed change log](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/blob/master/.github/temp/v2.54.13_v2.53.14_Detailed_change_log.txt)
---
## [v2.53.14](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.53.14)
#### Change log:
- New feature: [Add File] button now supports selecting and adding multiple files.
- New feature: Add [Ban Gitee] option, enabling this option will prevent the software from downloading files from Gitee.
- Update RealSR-ncnn-vulkan, Waifu2x-ncnn-vulkan, ImageMagick, Python extension.
- Performance optimization, reduce network traffic consumption and calls to external programs.
- Fix multiple bugs.
- [And many other improvements, click to view detailed change log](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/blob/master/.github/temp/v2.53.14_v2.52.16_Detailed_change_log.txt)
---
## [v2.52.16](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.52.16)
#### Change log:
- New feature: Add buttons to verify GPUs configuration for Anime4k & Waifu2x-caffe engine.
- Optimize SRMD-ncnn-vulkan engine to improve performance.
- Update ImageMagick, FFmpeg&FFprobe, waifu2x-caffe, Anime4k.
- Built-in cuDNN.
- Performance optimization.
- Fix multiple bugs.
- [And many other improvements, click to view detailed change log](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/blob/master/.github/temp/v2.52.16_v2.51.17_Detailed_change_log.txt)
---
## [v2.51.17](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.51.17)
#### Change log:
- New feature: Add Multi-GPU support for all engines.
- New feature: Add taskbar icon, support minimize to taskbar.
- New feature: Background mode.
- New feature: Multiple update channel (stable, beta).
- New feature: The original settings will be retained after the update.
- New feature: Add fast mode support for the ACNet algorithm of the Anime4k engine.
- New feature: ACNet algorithm supports Specify GPUs.
- New feature: Add overwrite switch.
- Update ImageMagick, waifu2x-ncnn-vulkan, FFmpeg.
- Performance optimization.
- Fix multiple bugs.
- [And many other improvements, click to view detailed change log](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/blob/master/.github/temp/v2.51.17_v2.45.18_Detailed_change_log.txt)
---
## [v2.45.18](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.45.18)
#### Change log:
- New feature: Add HDN mode support to the Anime4k engine to improve image quality. (HDN can only be enabled after ACNet is enabled)
- New feature: Keep original file name. (optional, disabled by default)
- Update Anime4K, ImageMagick, FFmpeg.
- New notification sound with fadeout.(Edited by @Michael18751)
- Performance optimization.
- Fix multiple bugs.
- And many other improvements.
---
## [v2.44.18](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.44.18)
#### Change log:
- New feature: Add ACNet algorithm support for Anime4K engine, ACNet can achieve high-speed processing while improving image quality.(You need to manually enable ACNet in the Anime4k engine settings)
- Update ImageMagick, waifu2x-ncnn-vulkan, SRMD-ncnn-Vulkan, realsr-ncnn-vulkan, Anime4K.
- Optimize performance and improve stability.
- Fixed multiple bugs.
- And many other improvements.
---
## [v2.43.17](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.43.17)
#### Change log:
- New feature: Pre-process Image. This will improve compatibility. (Additional settings, optional, disabled by default)
- Update Python extension,waifu2x-ncnn-vulkan,srmd-ncnn-vulkan,realsr-ncnn-vulkan,FFmpeg,ImageMagick.
- Improve the process of checking for update.
- Improve multi-thread scheduling mechanism.
- Add and modify tooltip.
- Support online update of donate QR code.
- Add some tips, modify some text, correct typos.
- Performance optimization.
- Fix several bugs.
- Other improvements.
---
## [v2.41.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.41.12)
#### Change log:
- #### New features: Add RealSR-ncnn-vulkan engine, greatly improving the ability to process 3D Real-life style images (thanks to @CAFUCSteven for assistance in testing software).
- New feature: All engines (except Anime4k) now support automatic recognition and processing of Alpha channel pictures.
- Update waifu2x-ncnn-vulkan engine.
- Update srmd-ncnn-vulkan engine.
- Update ImageMagick.
- Optimize the launcher.
- Optimize the process of checking for update.
- Adjust the processing flow for pictures with Alpha channel.
- Fixe several bugs.
- Other improvements.
---
## [v2.31.14](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.31.14)
#### Change log:
- New feature: Add waifu2x-caffe engine (experimental function) (thanks to @CAFUCSteven for assistance in testing the software).
- New feature: waifu2x-caffe engine supports quick switching of image styles.
- New feature: Support for switching the engine used when processing images with Alpha channels.
- Optimize the process of processing pictures with Alpha channel.
- Adjust the compatibility test interface.
- Performance optimization.
- Change default settings.
- Add some tips, modify some text, correct typos.
- Fix multiple bugs.
- Other improvements.
---
## [v2.21.12](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.21.12)
#### Change log:
- New feature: When processing video or GIF, the progress of the current file (a progress bar, Time cost, Time remaining, ETA) is displayed separately.
- Performance optimization.
- Improve the compatibility of ffporbe plugin.
- Fix bug: In some cases, the video processing will be stuck in the step of obtaining the duration.
- Other improvements.
---
## [v2.11.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.11.3)
#### Change log:
- New feature: Anime4K engine supports processing Image and GIF.
- New feature: Automatically adjust engine settings based on compatibility test results.
- After the compatibility test, a pop up will shows up according to the test results.
- Update Anime4K (v1.8.1).
- Update ImageMagick (7.0.10-12-Q16-x64).
- Change default settings.
- Add some tips.
- Check whether the software has write permission in the directory where the file is located before processing the file.
- Improved permission detection when the software starts.
- Fix bug: In special cases, the video may be stuck in the step of obtaining the duration.
- Fix bug: Can't detect whether the software has write permission for output path normally.
- Fix bug: when using Anime4k engine to process video, the custom resolution setting is invalid.
---
## [v2.02.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.02.3)
#### Change log:
- Update Anime4K (v1.7.0).
- Improve Simplified Chinese support.
- Reduce resource usage when running compatibility tests.
- Add some tips.
- Fix bug: In some cases, the program will get stuck when running compatibility tests.
- Fix bug: Some components are not disabled when processing files, which may cause potential errors.
---
## [v2.01.1](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v2.01.1)
#### Change log:
- New feature: Redesigned user interface.
- New feature: add [繁體中文] support (thanks @uimee for assistance in translation).
- New feature: Anime4K engine supports specified GPU.
- New feature: store and read GPU settings of all engines.
- New features: improved compatibility testing, increased inspection items, and support for storing test results.
- Update Anime4K (v1.6.0).
- Update ImageMagick (7.0.10-10-Q16-x64).
- Improved multi-thread management.
- Add some tips.
- Performance optimization.
- Fix bugs.
---
## [v1.73.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.73.3)
#### Change log:
- New feature: Add GPU acceleration support for Anime4K engine.
- New feature: After installing the software, a pop-up window allows users to choose their own language when they first start up.
- Update Anime4K (v1.5.0)
- It is no longer allowed to disable the automatic check for updates, but the automatic update pop-up window can be disabled. After disabling the pop-up window, an update prompt will be displayed in the text box.
- A pop-up window prompts the user to view the test results after the compatibility test.
- Improve compatibility test.
- Hide ETA and remaining time when GIF or video is included in the file list.
- Improve multi-language support.
- Fix bugs.
---
## [v1.71.1](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.71.1)
#### Change log:
- New feature: replaced the previous Anime4K-JAVA with Anime4KCPP.Anime4KCPP is faster and has better image quality than Anime4K-JAVA.
- New feature: Add a lot of custom settings for the Anime4K engine.
- Interface layout adjustment.
- Fixe translation errors.
- Modify some texts.
---
## [v1.63.1](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.63.1)
#### Change log:
- Improve stability.
- Optimize performance.
- Add some tips.
- Change some text.
- Fix translation errors.
- Fix bug: In rare cases, the cached files will have the same name and cause an error.
- Fix bug: Reset video settings button does not work properly.
---
## [v1.62.5](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.62.5)
#### Change log:
- Fix bug: when the `Process video by segment` is enabled, the cache cannot be read normally, which will cause the software unable to continue the previous progress.(Thanks to Esper Wang for feedback✔)
---
## [v1.62.4](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.62.4)
#### Change log:
- Fix bug: In some cases, the output video will be out of sync.(thanks to  @FITHRPG6 for feedback)
---
## [v1.62.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.62.3)
#### Change log:
- New feature: waifu2x-ncnn-vulkan adds fp16p support, which improves compatibility with some old drivers.
- Update waifu2x-ncnn-vulkan (version 20200414).
- Update ImageMagick (7.0.10-6-Q16-x64).
- Change the default custom resolution aspect ratio strategy to keep aspect ratio.
- Fixe bug: interface display error in some cases.
- Fixe bug: when the source video file name contains Chinese, the video cannot be assembled correctly after processing the video in segments.
---
## [v1.61.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.61.3)
#### Change log:
- New feature: Processing video in segments, greatly reducing the hard disk space occupied when processing video. 🎉🥳🎉 (Optional, additional settings, enabled by default)
- Improve multi-language support.
- Other minor improvements.
- Fix bug: When the processing process is stopped, the ffmpeg process will be forcibly terminated, which will cause the cache file cannot be generated normally.
- Fix bug: In some cases, the progress bar cannot display the progress normally.
---
## [v1.51.3](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.51.3)
#### Change log:
- Performance optimization.
- Remove redundant code.
- Improve multi-language support.
- Fix bug: When the software language is Japanese, the Readme cannot be opened normally.
- Fixed bug: Some cache files automatically generated by this software may be recognized as empty files by junk cleaning software and deleted.
- Fix bug: Inaccurate countdown time before shutdown.
- Other small improvements.
---
## [v1.50.2](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.50.2)
#### Change log:
- New feature: Use SoX (14.4.2-win32) to reduce the noise of the video's audio. (Optional, additional settings, disabled by default) (thanks @wenbob for the suggestion)
- New feature: Software settings will be saved before automatically shutting down the computer.
- Optimized interface display.
- Improve multi-language support and fix translation errors.
- Fix bug: When [Keep Video Cache] is enabled, the source video files will still be deleted.
---
## [v1.45](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.45)
#### Change log:
- New feature: You can choose whether to show a pop up when exit. (Optional, additional settings, enabled by default)
- New feature: Automatically enable(or disable) [Auto Detect Alpha Channel] based on the results of the compatibility test.
- New feature: Keep video cache. (Optional, additional settings, enabled by default)
- New feature: When the user stops the task or an error occurs, the video's cache will not be automatically deleted, and it can also be read by the software to continue the previous progress.
- Improve the stability of multi-threaded scheduling.
- Fix bug: In some cases, the file cannot be renamed properly then the video cannot be assembled normally.
- Fix bug: The files in the list could not be processed normally due to the thread scheduling error.
---
## [v1.37](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.37)
#### Change log:
- New feature: When converting videos to mp4, support to automatically obtain the bit rate of the original video and apply it to the converted mp4.
- New feature: When outputting video, the bit rate will be allocated using the software's built-in algorithm.
- Change the default [compressed ".jpg" image quality] value to 95.
- Fix bug: Progress bar could not display progress normally in some cases.
---
## [v1.31](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.31)
#### Change log:
- New feature: Automatically determine whether the picture has an alpha channel and switch to a compatible engine. (Optional, additional settings, disabled by default) (`Please make sure your computer is compatible with waiuf2x-converter before enabling this feature.`)
- New feature: Compatibility tests run automatically the first time the software is launched.
- Improved multi-thread management and stability.
- Remove the [Show Tips] button.
- Fix bug: In some cases, outputting the processor list of waifu2x-converter will cause the software to enter an endless loop.
---
## [v1.21](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.21)
#### Change log:
- New feature: support remember the last browsed folder
- New feature: Improved automatic check for updates, support for displaying update logs
- New feature: Launcher added multi-open detection.
- New feature: Support for typing extra commands in video customization settings.
- Update ImageMagick (7.0.9-27-Q16-x64)
- Update User-Agent used when checking for updates automatically.
- Changed some interface layouts.
- Improved stability.
- Added some tips.
- Modified some confusing text.
---
## [v1.11](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.11)
#### Change log:
- New feature: Add SRMD-NCNN-Vulkan engine. 🎉🥳🎉
The SRMD-NCNN-Vulkan engine can support both `2D Anime` and `3D Real-life` image styles.
You can [click this page](https://github.com/cszn/SRMD) to learn about SRMD.
---
## [v1.01](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v1.01)
#### Change log:
- ### End the beta test and start the development of the stable version. 🎉🥳🎉
- New feature: Add [ 日本語 Japanese ] language support.  🐱‍👤
`(Machine translation, may contain errors)`
- Added some tips.
- Fix bug: text error.
- Fixed bug: After switching languages, some texts were displayed incorrectly.
---
## [v0.57-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.57-beta)
#### Change log:
- Add PayPal donate button
- Rewrite code related to file list to speed up operation and reduce memory consumption.
- Fix bug: When there are many entries in the list, removing a single entry will cause no response.
- Fix bug: After specifying the output path, files with the same file name will overwrite each other.
- Fix bug: New and old versions of waifu2x-ncnn-vulkan are not distinguished when detecting available GPU ID
---
## [v0.56-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.56-beta)
#### Change log:
- Fix bug: slow reading files speed
- Fix bug: unable to stop processing file process normally due to waiting for ffmpeg to split video (or GIF)
- Fix bug: In some cases, external plugins are still running when exiting the program
---
## [v0.55-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.55-beta)
#### Change log:
- Old version of waifu2x-ncnn-vulkan engine is enabled by default. (Because of the stability issue of new version of waifu2x-ncnn-vulkan)
`If you need to use the TTA feature of the waifu2x-ncnn-vulkan engine, switch to the new version.`
- Improve stability.
- Fix bug: Adding a large number of files at one time will cause the program to become unresponsive.
---
## [v0.54-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.54-beta)
#### Change log:
- New feature: When the software is closed, a pop-up window asks the user whether to confirm the exit.
- New feature: Added [Forced Retry], when waifu2x thread is stuck, you can perform forced retry to remove the stuck, and it will not interrupt the entire [scale and denoise] process
- Improve error detection of waifu2x-ncnn-vulkan engine.
- Fix bug: not delete all temporary files in some cases
- Fix bug: In some special cases, multi-threaded scheduling error will cause stuck
---
## [v0.53-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.53-beta)
#### Change log:
- New feature: Support switching waifu2x-ncnn-vulkan engine version. When your computer has problems using waifu2x-ncnn-vulkan engine, you can try to update the graphics card driver or enable the old version of waifu2x-ncnn-vulkan engine
- New feature: Added compatibility test for older versions of waifu2x-ncnn-vulkan engine
- New feature: Custom retry times (additional settings)
- Try to fix the problem of high DPI screen display. (I cannot test because I don’t have a high DPI display myself)
- Fix bug: text error
---
## [v0.52-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.52-beta)
#### Change log:
- Improved stability, will retry when the engine crashes, and will not fail the entire process because of an engine crash
- Improve the stability of Anime4k engine
- Disable lineEdit of output path when output path is not enabled
- Fix text errors
- Update waifu2x-ncnn-vulkan (version 20200224)
---
## [v0.51-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.51-beta)
#### Change log:
- New feature: When "Delete original file" is enabled, you can choose to move the original file to the recycle bin
- New feature: Support to choose whether to enable custom video settings (additional settings, optional, disabled by default)
- New feature: Specify output directory
- New feature: Scan subfolders (additional settings, optional, enabled by default)
- New feature: Added TTA support for waifu2x-ncnn-vulkan engine
- New feature: Added TTA support for waifu2x-converter engine
- New feature: file list interactivity settings (additional settings)
- Update waifu2x-ncnn-vulkan (20200223)
- Performance optimization
- Improve error detection
- Fix bug: text error
---
## [v0.461-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.461-beta)
#### v0.461-beta Change log:
- Fix bug: Source video files may get lost in some cases
#### v0.46-beta Change log:
- New feature: Support for more video-related custom parameters
- New feature: Show prompts on initial startup
- Update waifu2x-ncnn-vulkan (20200222)
- Interface layout adjustment
- Enhance video quality
- Fix bug: Temporary mp4 video generated by software was not deleted when processing stopped
- Fix bug: When waifu2x-ncnn-vulkan is enabled, the target magnification cannot be calculated correctly (thanks to slimekingwin8cn for feedback)
---
## [v0.45-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.45-beta)
#### Change log:
- New feature: waifu2x-ncnn-vulkan engine supports switching to cunet model
- New feature: custom video encoder, bitrate and pixel format (in additional settings)
- New feature: Custom resolution supports apply settings to all files together
- Enhanced video quality
- Performance optimization, reducing the time required to process GIF and video when custom resolution is enabled
- Fix bug: target magnification cannot be calculated correctly when custom resolution is enabled
---
## [v0.411-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.411-beta)
#### v0.411 Change log:
- Improve compatibility of waifu2x-converter
#### v0.41 Change log:
- New feature: waifu2x-converter supports more noise reduction levels
- New feature: Added waifu2x-converter engine custom settings
- New feature: custom font
- New feature: minimize form
- New feature: hide text browser
- Update waifu2x-converter (v5.3.3) (thanks to NyanMisaka for feedback)
- Interface layout adjustment
- Improve stability
- Many other improvements
- Fix bug: File extensions are not recognized correctly (thanks to zhehenkaifa for feedback)
- Fix bug: When the video extension is ".MP4" instead of ".mp4", it will cause an error
- Fix bug: error caused by extra "." In file name (thanks to 我叫黄伟达 for feedback)
- Fix bug: unable to stop processing in some special cases
---
## [v0.37-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.37-beta)
#### Change log:
- New feature: Custom ".jpg" file compressed image quality
- Improve file extension filtering in browse file dialog
- Update ImageMagick (7.0.9-22-Q16-x64)
- Improve stability
- Improve Simplified Chinese support
- Other small improvements
- Fix bug: stuck in the background after the program is closed
---
## [v0.35-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.35-beta)
#### Change log:
- New feature: Custom global font size (additional settings)
- New feature: Browse and add files
- Performance optimization
- Improve stability
- Review code and add code comments
- Interface layout adjustment
- Multiple minor improvements
- Fix bug: Cannot be compatible with custom scaling of Windows system
- Fix bug: In some special cases, it can't judge whether the file is added repeatedly
- Fix bug: Can't save noise reduction level setting
---
## [v0.31-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.31-beta)
#### Change log:
- New feature: show progress while loading file list
- New feature: Customizable aspect ratio strategy of "Custom Resolution" (in [Additional Settings])
- New feature: popup prompt after manually saving settings
- New feature: "Settings" can always be hidden (optional, disabled by default, in [Additional Settings])
- New feature: Show total number of GIF and video threads
- Fine-tune interface layout
- Fix bug: When processing gif, the file processing status cannot be changed normally after stopping the process
---
## [v0.291-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.291-beta)
#### Change log:
- New feature: Automatically save settings when closing the program (optional, enabled by default)
- New feature: [input path] can be hidden all the time (optional, disabled by default)
- New feature: Add [About]
- New feature: Permission detection
- Adjust the interface layout, move some setting options to [Additional settings]
- Improve Simplified Chinese support
- Fix bug: In some special cases, the program will be stuck in the background
---
## [v0.281-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.281-beta)
#### Change log:
- New feature: [Files List] supports deselect
- Interface Beautification
- Adjust interface layout
- Improve Simplified Chinese support
- Fix bug: GIF frames could not be arranged properly in some cases
- Fix bug: In some cases, the thread will be automatically closed in advance and the task cannot be completed
- Fix bug: In some cases, the program cannot exit completely and will stay in the background to execute an infinite loop
- Fix bug: When there is no Java runtime environment in the system, calling Anime4k may cause the software to enter an infinite loop
---
## [v0.25-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.25-beta)
#### Change log:
- New feature: Read screen resolution and set as default custom resolution value when first started
- New feature: When loading File List, automatically output items with status [Failed] in Textbrowser
- Update FFmpeg (4.2.2)
- Fix bug: In some special cases, automatic check for updates will falsely report the existence of a new version
- Fix bug: Automatic shutdown of computer could not be performed normally
- Fixed bug: [File Count] cannot be displayed normally after language switching
- Improve Simplified Chinese language support
---
## [v0.21-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.21-beta)
#### Change log:
- New feature: [Completed number of files/Total number of files] is displayed on the left side of the progress bar.
- New feature: Added setting options to control whether to automatically check for updates at startup (It is `not recommended` to turn off automatic updates)
- New feature: The total number of files is displayed below the file list.
- New feature: Save/Read file list
- New feature: Automatically save the file list before automatically shutting down the computer,  you can manually load the file list to check the file processing status after the next software startup
- New feature: pop-up window prompt before auto shutdown
- Improve Simplified Chinese language support
- Select the readme to open based on the current language
- Before processing a file, check if it exists
- Fix bug: After saving the settings, the [Image Style] settings that were saved cannot be read normally
- Fix bug: After removing a single row, the custom resolution settings of all remaining rows will be cleared
- Fix bug: When there are files with the same file name and different extensions in the file list, if multi-threading is enabled, it will cause read and write conflicts.
- Fix bug: The problem that the new version download page cannot be opened normally after detecting the new version automatically.
---
## [v0.12-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.12-beta)
#### Change log:
- NEW Feature: Check for updates automatically.
- Fix bug: GIF and video cannot read the scale ratio setting normally.
- Fix bug: When processing videos and gif files, if an error occurs, it will cause thread management problems.
---
## [v0.11-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.11-beta)
#### Change log:
- NEW Feature: Customize the resolution of image, GIF and video output. (At the request of an anonymous donor.🧐)
- NEW Feature: Multi-language.(Add Simplified Chinese.)(At the request of an anonymous donor.🧐)
- NEW Feature: Support to save the current settings, automatically restore the last saved settings when starting the software.
- NEW Feature: Switch the display status of setting options. (Hide / Show)
- NEW Feature: Switch the display status of [Input]. (Hide / Show)
- NEW Feature: Prompt when misoperation.
- NEW Feature: Automatically scroll to the bottom after changing the font size of Textbrowser.
- NEW Feature: Textbrowser automatically slides to the bottom after outputting new content
- NEW Feature: Tableview automatically adjusts sieze based on content
- NEW Feature: Check available GPU and set GPU ID.
- Improve tableview selection logic. When one tableview is selected, the other two are automatically unselected.
- Optimize the tableview display logic. After inputting the file, only change the display state of the corresponding tableview.
- Remove redundant code
- Fix bug: [Remove item] will cause the program to crash when the file is finished and [Re-process finished files] is not enabled.
- Fix bug: [video_gif_info.exe] Chinese characters cannot be read normally
- Fix bug: [Compatibility check] button is not automatically enabled after all files have been processed.
---
## [v0.01-beta](https://github.com/AaronFeng753/Waifu2x-Extension-GUI/releases/tag/v0.01-beta)
#### Change log:
- First release.

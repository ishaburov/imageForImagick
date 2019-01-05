# imageForImagick
class Image for Imagick
use 
  -----------------------------
            $image = new Image($yourImage);
           
           switch ($resize_method) {
								case 1:
									$image->resize($thumb_width, $thumb_height)->saveToPath(FILES_DIR.$dir."/thumb/".$file_name, 85);
									break;
								case 2:
									$image->resizeByWidth($thumb_width)->saveToPath(FILES_DIR.$dir."/thumb/".$file_name, 85);
									break;
								case 3:
									$image->resizeFitTo($thumb_width, $thumb_height)->saveToPath(FILES_DIR.$dir."/thumb/".$file_name, 85);
									break;
							}
						$image->reset();
						$image->saveToPath($path, $quality);

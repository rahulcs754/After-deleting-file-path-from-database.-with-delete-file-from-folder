# After-deleting-file-path-from-database.-with-delete-file-from-folder
After deleting file path from database. with delete file from folder

```php
    $path = './uploads/property/';
		
		$wheref = array('sno'=>$id);
		$image =  $this->Common_Model->select_data('property_images',' ',$wheref);

		if(file_exists($path.$image[0]->image_name))
		{
			@unlink($path.$image[0]->image_name);
		}

```

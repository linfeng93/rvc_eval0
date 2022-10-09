# rvc_eval0
The Validity Evaluation for RVC 2022

the predicted object detection results using our full unified label space

the zipped file includes
- eval0.test.json
    store the resulting detections in COCO submission format:
      json with list of dicts per detection with 
        {'image_id':<filename>, 'bbox':[x0_pxl,y0_pxl,w_pxl,h_pxl], 'score':<confidence_between_0_and_1>, 'category_id':<cat_id>}
      
- eval0_boxable.rvc_test.json
    store the input images info in COCO format:
      json with list of dicts per image with
        {'file_name':<filename>, 'id':<image_id>, 'width':<img_w>, 'height':<img_h>}
    store the category info in COCO format:
      json with list of dicts per category with
        {'supercategory':'rvc_jls', 'id':<cat_id>, 'name':<cat_name>}

- obj_det_mapping_v2.csv
    store the mappings from unified category names <cat_name> into each of the respective dataset category names
  
- unified2coco.json
    store the mappings from unified category ids <cat_id> into COCO dataset category ids
  
- unified2mvd.json
    store the mappings from unified category ids <cat_id> into MVD dataset category ids
  
- unified2oid.json
    store the mappings from unified category ids <cat_id> into OID dataset category ids

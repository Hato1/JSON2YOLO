# Databolt json -> YOLO4 Converter 

This is my branch of a json2yolo script that's been adjusted to accept Databolt-style json file. Databolt's annotations to yolo4 format. Input is a single json file downloaded from https://app.databolt.ai, output is a yolo4 text file for every image.

### HOW TO USE:

1. Place an input file (EG: exported-211125T082923.json) into the input directory. 
2. Run general_json2yolo.py.
3. Collect the output in the output directory. 
4. Verify the output is OK (I use YoloLabel and LabelIMG to verify annotations)

#### Caution:

* Old output may be deleted.
* Class numbering isn't fixed. (Forklift could be either class 0 or class 1 in a two class project) Be sure to make forklift class 0 and worker class 1 to avoid complications later down the line  (EG: Victors 3m_rule_metric).
* If the script fails, it can be the input that has an error.
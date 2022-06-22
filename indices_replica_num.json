# Change all the current index's to one replica - 

PUT /*/_settings
{
 "index" : {
  "number_of_replicas":0,
  "auto_expand_replicas": false
 }
}


Change all the upcoming index's -

PUT _index_template/all_indices
{
  "index_patterns": [
    "*"
  ],
  "priority": 0,
  "template": {
    "settings": {
      "number_of_replicas": 0
    }
  }
}

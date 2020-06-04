## TigXLNet

TigXLNet is XLNet based transformer model for low-resource language Tigrinya (a language in East Africa mainly used in Eritrea and Ethiopia). The model is trained using a corpus collected from different online platforms including Tigrinya news portals, social media posts, and few Tigrinya ebooks.  

Note try to load the model by setting the config file as follows:

      config = AutoConfig.from_pretrained("abryee/TigXLNet")
      config.d_head = 64 #To avoid a bug in loading d_head from config file.
      model = AutoModel.from_pretrained("abryee/TigXLNet", config=config)

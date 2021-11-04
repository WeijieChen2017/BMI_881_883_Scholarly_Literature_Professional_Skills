Hello everyone, this is Weijie Chen from the Univerisity of Wisconsin-Madison. Today I want to share the progress on PET/CT attenuation corrections. 

As we know, patients are moving and breathing. So PET and sCT may have some unregistered signals in some areas, like the lung-liver boundary. Intuitively, we want to generate an accurate attenuation map by combining sCT and PET. However, it is hard to acquire both registered and unregistered sCT at the same time, for the training pairs. 

So some methods will manually create sCT with deformations and teach the model to restore the distortion. Of course, this method is artificial and can not cover all possible mismatches. 

Here we proposed a vision transformer model to directly synthesize a pseudo-sCT from PET and register real sCT to it. The vision transformer model will divide the input images into patches and translate this sequence into the target domain with the help of the self-attention mechanism. 

By doing this, we have a great pipeline to have attenuation corrected PET images, without the influence of respiration and patient's movement. Thank you!

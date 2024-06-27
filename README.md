!pip install pygit2==1.12.2
%cd /content
!git clone https://github.com/lllyasviel/fooocus.git

%cd /content/Fooocus/model/upscale models/
!wget -0 fooocus_upscaler_s409985e5.bin https://huggingface.co/lllyasviel/misc/resolve/main/fooocus_uspcaler_s409985e5.bin?download=true

%cd /content/fooocus
!python entry_with_update.py --share

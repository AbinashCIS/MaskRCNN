1. change env/lib/python3.6/site-packages/keras/engine/topology.py at line 3114
from :  
if 'keras_version' in f.attrs:
        original_keras_version = f.attrs['keras_version'].decode('utf8')
    else:
        original_keras_version = '1'
    if 'backend' in f.attrs:
        original_backend = f.attrs['backend'].decode('utf8')
    else:
        original_backend = None

To : 

if 'keras_version' in f.attrs:
        original_keras_version = f.attrs['keras_version]
    else:
        original_keras_version = '1'
    if 'backend' in f.attrs:
        original_backend = f.attrs['backend']
    else:
        original_backend = None


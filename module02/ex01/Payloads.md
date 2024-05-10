# -*- coding: utf-8 -*-

import pickle
import base64

comando = "cat /etc/passwd"

serialized = (pickle.dumps(comando))

#Conversão do fluxo de bytes serializados para base64
serialized64 = base64.b64encode(serialized)


print('\n'+'Object serialized in base64:', serialized64.decode(),'\n')

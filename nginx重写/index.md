# Nginx重写


`  if ($uri ~* "/bankH5/.*yh/(.*)"){
            rewrite ^/bankH5/.*yh/(.*) /bankH5/$1 break;
        }
        if ($uri ~* "/bankH5/.*zncs/(.*)"){
            rewrite ^/bankH5/.*zncs/(.*) /bankH5/$1 break;
        }
        if ($uri ~* "/yszc/.*qyzc/(.*)"){
            rewrite ^/yszc/.*qyzc/(.*) /yszc/$1 break;
        }`


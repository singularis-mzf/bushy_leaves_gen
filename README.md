# bushy_leaves_gen

Generator script for bushy_leaves mod

## How to use

To generate the full model:

``perl -CSDAL -I. -Mv5.26.0 -Mstrict -Mwarnings -Mutf8 -MEnglish -MLinuxKnihaKouzel model.pl > bushy_leaves_full_model.obj``

To generate the cheap model:

``sed -i -E '/^my \$full_model =/s/1/0/' model.pl``
``perl -CSDAL -I. -Mv5.26.0 -Mstrict -Mwarnings -Mutf8 -MEnglish -MLinuxKnihaKouzel model.pl > bushy_leaves_cheap_model.obj``

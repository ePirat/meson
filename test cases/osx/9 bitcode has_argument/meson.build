project('bitcode has_argument test', 'c',
    default_options : ['b_bitcode=true'])

cc = meson.get_compiler('c')

# The -mstack-alignment= flag is not compatible with
# -fembed-bitcode, so this should not succeed.
assert(not cc.has_argument('-mstack-alignment=16'))

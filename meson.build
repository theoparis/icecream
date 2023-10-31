project('icecream', 'c', 'cpp')

configuration_inc = include_directories('.')

conf_data = configuration_data()
conf_data.set('version', '0.0.1')
conf_data.set('HAVE_ARPA_NAMESER_H', false)
conf_data.set('HAVE_SYS_SOCKETVAR_H', false)
conf_data.set('HAVE_IFR_DSTADDR', false)
conf_data.set('HAVE_LIBARCHIVE_ZSTD', true)
conf_data.set('HAVE_LIBARCHIVE_XZ', false)
configure_file(
  input: 'config.h.in',
	output: 'config.h',
	configuration: conf_data
)

subdir('services')
subdir('scheduler')
subdir('client')
subdir('compilerwrapper')
subdir('daemon')


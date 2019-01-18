load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'cppcoro',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '**/*.hpp'),
  ]),
  headers = subdir_glob([
    ('lib', '**/*.hpp'),
  ]),
  srcs = [
    'lib/async_auto_reset_event.cpp',
    'lib/async_manual_reset_event.cpp',
    'lib/async_mutex.cpp',
    'lib/cancellation_state.cpp',
    'lib/cancellation_token.cpp',
    'lib/cancellation_source.cpp',
    'lib/cancellation_registration.cpp',
    'lib/lightweight_manual_reset_event.cpp',
    'lib/ip_address.cpp',
    'lib/ip_endpoint.cpp',
    'lib/ipv4_address.cpp',
    'lib/ipv4_endpoint.cpp',
    'lib/ipv6_address.cpp',
    'lib/ipv6_endpoint.cpp',
    'lib/static_thread_pool.cpp',
    'lib/auto_reset_event.cpp',
    'lib/spin_wait.cpp',
    'lib/spin_mutex.cpp',
  ],
  # srcs = glob([
    # 'lib/**/*.cpp',
  # ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)

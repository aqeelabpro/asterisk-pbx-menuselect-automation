# Asterisk PBX Make MenuSelect programmatically

**Overview:**
The menuselect/menuselect utility is a command-line interface tool designed to manage the configuration options for software components, particularly focusing on enabling or disabling specific options and categories within a menu-driven selection interface.

**Usage:**
The menuselect/menuselect utility supports several command-line options to facilitate the configuration process. Below is a detailed explanation of each option:

1. **--enable <option>:**
   - This option allows the user to enable a specific configuration option.
   - Example: `menuselect/menuselect --enable <option>`
   - Example from Asterisk PBX `menuselect/menuselect --enable app_macro`

2. **--disable <option>:**
   - This option allows the user to disable a specific configuration option.
   - Example: `menuselect/menuselect --disable <option>`
   - Example from Asterisk PBX `menuselect/menuselect --disable app_macro`

3. **--enable-category <category>:**
   - Enables all options within the specified category.
   - Example: `menuselect/menuselect --enable-category <category>`

4. **--enable-all:**
   - Enables all configuration options.
   - Example: `menuselect/menuselect --enable-all`

5. **--disable-category <category>:**
   - Disables all options within the specified category.
   - Example: `menuselect/menuselect --disable-category <category>`

6. **--disable-all:**
   - Disables all configuration options.
   - Example: `menuselect/menuselect --disable-all`

7. **--list-options:**
   - Lists all available configuration options.
   - Example: `menuselect/menuselect --list-options`

8. **--list-category <category>:**
   - Lists options within the specified category.
   - Example: `menuselect/menuselect --list-category <category>`

9. **--category-list:**
    - Lists all available categories.
    - Example: `menuselect/menuselect --category-list`

10. **--help:**
    - Displays usage information.
    - Example: `menuselect/menuselect --help`

**Additional Information:**
- The `<config-file>` parameter is optional and represents the configuration file(s) to be processed.
- Multiple options and categories can be specified in a single command.
- Options and categories should be provided with their respective names.
- The utility provides flexibility in enabling/disabling options and categories, listing available options/categories, and checking dependencies.

**Examples:**
1. Enable the option `example_option`:
   ```
   menuselect --enable app_macro
   ```

2. Disable the option `example_option`:
   ```
   menuselect --disable app_macro
   ```

3. Enable all options within the category `MENUSELECT_APPS`:
   ```
   menuselect --enable-category MENUSELECT_APPS
   ```

4. Enable all options:
   ```
   menuselect --enable-all
   ```

5. List all available options:
   ```
   menuselect/menuselect --list-options
   ```
   ### Example Output: 
 
         Option                                             Category                
         chan_mobile                                        MENUSELECT_ADDONS       
         chan_ooh323                                        MENUSELECT_ADDONS       
         format_mp3                                         MENUSELECT_ADDONS       
         res_config_mysql                                   MENUSELECT_ADDONS       
         app_mysql                                          MENUSELECT_ADDONS       
         cdr_mysql                                          MENUSELECT_ADDONS       
         app_agent_pool                                     MENUSELECT_APPS         
         app_authenticate                                   MENUSELECT_APPS         
         app_bridgeaddchan                                  MENUSELECT_APPS         
         app_bridgewait                                     MENUSELECT_APPS         
         app_cdr                                            MENUSELECT_APPS         
         app_celgenuserevent                                MENUSELECT_APPS         
         app_channelredirect                                MENUSELECT_APPS         
         app_chanspy                                        MENUSELECT_APPS         
         app_confbridge                                     MENUSELECT_APPS         
         app_controlplayback                                MENUSELECT_APPS         
         app_db                                             MENUSELECT_APPS         
         app_dial                                           MENUSELECT_APPS         
         app_directed_pickup                                MENUSELECT_APPS         
         app_directory                                      MENUSELECT_APPS         
         app_disa                                           MENUSELECT_APPS         
         app_dumpchan                                       MENUSELECT_APPS         
         app_echo                                           MENUSELECT_APPS         
         app_exec                                           MENUSELECT_APPS         
         app_flash                                          MENUSELECT_APPS         
         app_followme                                       MENUSELECT_APPS         
         app_forkcdr                                        MENUSELECT_APPS         
         app_milliwatt                                      MENUSELECT_APPS         
         app_mixmonitor                                     MENUSELECT_APPS         
         app_originate                                      MENUSELECT_APPS         
         app_page                                           MENUSELECT_APPS         
         app_playback                                       MENUSELECT_APPS         
         app_playtones                                      MENUSELECT_APPS         
         app_privacy                                        MENUSELECT_APPS         
         app_queue                                          MENUSELECT_APPS         
         app_read                                           MENUSELECT_APPS         
         app_readexten                                      MENUSELECT_APPS         
         app_record                                         MENUSELECT_APPS         
         app_sayunixtime                                    MENUSELECT_APPS         
         app_senddtmf                                       MENUSELECT_APPS         
         app_sendtext                                       MENUSELECT_APPS         
         app_skel                                           MENUSELECT_APPS         
         app_softhangup                                     MENUSELECT_APPS         
         app_speech_utils                                   MENUSELECT_APPS         
         app_stack                                          MENUSELECT_APPS         
         app_stasis                                         MENUSELECT_APPS         
         app_stream_echo                                    MENUSELECT_APPS         
         app_system                                         MENUSELECT_APPS         
         app_talkdetect                                     MENUSELECT_APPS         
         app_transfer                                       MENUSELECT_APPS         
         app_userevent                                      MENUSELECT_APPS         
         app_verbose                                        MENUSELECT_APPS         
         app_voicemail                                      MENUSELECT_APPS         
         app_voicemail_imap                                 MENUSELECT_APPS         
         app_voicemail_odbc                                 MENUSELECT_APPS         
         app_waituntil                                      MENUSELECT_APPS         
         app_while                                          MENUSELECT_APPS         
         app_alarmreceiver                                  MENUSELECT_APPS         
         app_amd                                            MENUSELECT_APPS         
         app_attended_transfer                              MENUSELECT_APPS         
         app_audiosocket                                    MENUSELECT_APPS         
         app_blind_transfer                                 MENUSELECT_APPS         
         app_broadcast                                      MENUSELECT_APPS         
         app_chanisavail                                    MENUSELECT_APPS         
         app_dictate                                        MENUSELECT_APPS         
         app_dtmfstore                                      MENUSELECT_APPS         
         app_externalivr                                    MENUSELECT_APPS         
         app_festival                                       MENUSELECT_APPS         
         app_if                                             MENUSELECT_APPS         
         app_ivrdemo                                        MENUSELECT_APPS         
         app_jack                                           MENUSELECT_APPS         
         app_meetme                                         MENUSELECT_APPS         
         app_mf                                             MENUSELECT_APPS         
         app_minivm                                         MENUSELECT_APPS         
         app_morsecode                                      MENUSELECT_APPS         
         app_mp3                                            MENUSELECT_APPS         
         app_osplookup                                      MENUSELECT_APPS         
         app_reload                                         MENUSELECT_APPS         
         app_saycounted                                     MENUSELECT_APPS         
         app_sf                                             MENUSELECT_APPS         
         app_signal                                         MENUSELECT_APPS         
         app_sms                                            MENUSELECT_APPS         
         app_statsd                                         MENUSELECT_APPS         
         app_test                                           MENUSELECT_APPS         
         app_waitforcond                                    MENUSELECT_APPS         
         app_waitforring                                    MENUSELECT_APPS         
         app_waitforsilence                                 MENUSELECT_APPS         
         app_zapateller                                     MENUSELECT_APPS         
         app_adsiprog                                       MENUSELECT_APPS         
         app_dahdiras                                       MENUSELECT_APPS         
         app_fax                                            MENUSELECT_APPS         
         app_getcpeid                                       MENUSELECT_APPS         
         app_ices                                           MENUSELECT_APPS         
         app_image                                          MENUSELECT_APPS         
         app_macro                                          MENUSELECT_APPS         
         app_nbscat                                         MENUSELECT_APPS         
         app_url                                            MENUSELECT_APPS         
         bridge_builtin_features                            MENUSELECT_BRIDGES      
         bridge_builtin_interval_featur MENUSELECT_BRIDGES                          
         bridge_holding                                     MENUSELECT_BRIDGES      
         bridge_native_rtp                                  MENUSELECT_BRIDGES      
         bridge_simple                                      MENUSELECT_BRIDGES      
         bridge_softmix                                     MENUSELECT_BRIDGES      
         binaural_rendering_in_bridge_s MENUSELECT_BRIDGES                          
         cdr_adaptive_odbc                                  MENUSELECT_CDR          
         cdr_custom                                         MENUSELECT_CDR          
         cdr_manager                                        MENUSELECT_CDR          
         cdr_beanstalkd                                     MENUSELECT_CDR          
         cdr_csv                                            MENUSELECT_CDR          
         cdr_odbc                                           MENUSELECT_CDR          
         cdr_pgsql                                          MENUSELECT_CDR          
         cdr_radius                                         MENUSELECT_CDR          
         cdr_sqlite3_custom                                 MENUSELECT_CDR          
         cdr_tds                                            MENUSELECT_CDR          
         cdr_syslog                                         MENUSELECT_CDR          
         cel_custom                                         MENUSELECT_CEL          
         cel_manager                                        MENUSELECT_CEL          
         cel_odbc                                           MENUSELECT_CEL          
         cel_beanstalkd                                     MENUSELECT_CEL          
         cel_pgsql                                          MENUSELECT_CEL          
         cel_radius                                         MENUSELECT_CEL          
         cel_sqlite3_custom                                 MENUSELECT_CEL          
         cel_tds                                            MENUSELECT_CEL          
         chan_bridge_media                                  MENUSELECT_CHANNELS     
         chan_dahdi                                         MENUSELECT_CHANNELS     
         chan_iax2                                          MENUSELECT_CHANNELS     
         chan_motif                                         MENUSELECT_CHANNELS     
         chan_pjsip                                         MENUSELECT_CHANNELS     
         chan_rtp                                           MENUSELECT_CHANNELS     
         chan_alsa                                          MENUSELECT_CHANNELS     
         chan_audiosocket                                   MENUSELECT_CHANNELS     
         chan_console                                       MENUSELECT_CHANNELS     
         chan_mgcp                                          MENUSELECT_CHANNELS     
         chan_skinny                                        MENUSELECT_CHANNELS     
         chan_unistim                                       MENUSELECT_CHANNELS     
         chan_misdn                                         MENUSELECT_CHANNELS     
         chan_nbs                                           MENUSELECT_CHANNELS     
         chan_oss                                           MENUSELECT_CHANNELS     
         chan_phone                                         MENUSELECT_CHANNELS     
         chan_sip                                           MENUSELECT_CHANNELS     
         chan_vpb                                           MENUSELECT_CHANNELS     
         codec_a_mu                                         MENUSELECT_CODECS       
         codec_adpcm                                        MENUSELECT_CODECS       
         codec_alaw                                         MENUSELECT_CODECS       
         codec_codec2                                       MENUSELECT_CODECS       
         codec_dahdi                                        MENUSELECT_CODECS       
         codec_g722                                         MENUSELECT_CODECS       
         codec_g726                                         MENUSELECT_CODECS       
         codec_gsm                                          MENUSELECT_CODECS       
         codec_ilbc                                         MENUSELECT_CODECS       
         codec_lpc10                                        MENUSELECT_CODECS       
         codec_resample                                     MENUSELECT_CODECS       
         codec_speex                                        MENUSELECT_CODECS       
         codec_ulaw                                         MENUSELECT_CODECS       
         codec_opus                                         MENUSELECT_CODECS       
         codec_silk                                         MENUSELECT_CODECS       
         codec_siren7                                       MENUSELECT_CODECS       
         codec_siren14                                      MENUSELECT_CODECS       
         codec_g729a                                        MENUSELECT_CODECS       
         format_g719                                        MENUSELECT_FORMATS      
         format_g723                                        MENUSELECT_FORMATS      
         format_g726                                        MENUSELECT_FORMATS      
         format_g729                                        MENUSELECT_FORMATS      
         format_gsm                                         MENUSELECT_FORMATS      
         format_h263                                        MENUSELECT_FORMATS      
         format_h264                                        MENUSELECT_FORMATS      
         format_ilbc                                        MENUSELECT_FORMATS      
         format_ogg_vorbis                                  MENUSELECT_FORMATS      
         format_pcm                                         MENUSELECT_FORMATS      
         format_siren14                                     MENUSELECT_FORMATS      
         format_siren7                                      MENUSELECT_FORMATS      
         format_sln                                         MENUSELECT_FORMATS      
         format_wav                                         MENUSELECT_FORMATS      
         format_wav_gsm                                     MENUSELECT_FORMATS      
         format_ogg_speex                                   MENUSELECT_FORMATS      
         format_vox                                         MENUSELECT_FORMATS      
         func_aes                                           MENUSELECT_FUNCS        
         func_base64                                        MENUSELECT_FUNCS        
         func_blacklist                                     MENUSELECT_FUNCS        
         func_callcompletion                                MENUSELECT_FUNCS        
         func_callerid                                      MENUSELECT_FUNCS        
         func_cdr                                           MENUSELECT_FUNCS        
         func_channel                                       MENUSELECT_FUNCS        
         func_config                                        MENUSELECT_FUNCS        
         func_curl                                          MENUSELECT_FUNCS        
         func_cut                                           MENUSELECT_FUNCS        
         func_db                                            MENUSELECT_FUNCS        
         func_devstate                                      MENUSELECT_FUNCS        
         func_dialgroup                                     MENUSELECT_FUNCS        
         func_dialplan                                      MENUSELECT_FUNCS        
         func_enum                                          MENUSELECT_FUNCS        
         func_env                                           MENUSELECT_FUNCS        
         func_extstate                                      MENUSELECT_FUNCS        
         func_global                                        MENUSELECT_FUNCS        
         func_groupcount                                    MENUSELECT_FUNCS        
         func_hangupcause                                   MENUSELECT_FUNCS        
         func_holdintercept                                 MENUSELECT_FUNCS        
         func_iconv                                         MENUSELECT_FUNCS        
         func_jitterbuffer                                  MENUSELECT_FUNCS        
         func_lock                                          MENUSELECT_FUNCS        
         func_logic                                         MENUSELECT_FUNCS        
         func_math                                          MENUSELECT_FUNCS        
         func_md5                                           MENUSELECT_FUNCS        
         func_module                                        MENUSELECT_FUNCS        
         func_odbc                                          MENUSELECT_FUNCS        
         func_periodic_hook                                 MENUSELECT_FUNCS        
         func_pjsip_aor                                     MENUSELECT_FUNCS        
         func_pjsip_contact                                 MENUSELECT_FUNCS        
         func_pjsip_endpoint                                MENUSELECT_FUNCS        
         func_presencestate                                 MENUSELECT_FUNCS        
         func_rand                                          MENUSELECT_FUNCS        
         func_realtime                                      MENUSELECT_FUNCS        
         func_sha1                                          MENUSELECT_FUNCS        
         func_shell                                         MENUSELECT_FUNCS        
         func_sorcery                                       MENUSELECT_FUNCS        
         func_speex                                         MENUSELECT_FUNCS        
         func_sprintf                                       MENUSELECT_FUNCS        
         func_srv                                           MENUSELECT_FUNCS        
         func_strings                                       MENUSELECT_FUNCS        
         func_sysinfo                                       MENUSELECT_FUNCS        
         func_talkdetect                                    MENUSELECT_FUNCS        
         func_timeout                                       MENUSELECT_FUNCS        
         func_uri                                           MENUSELECT_FUNCS        
         func_version                                       MENUSELECT_FUNCS        
         func_vmcount                                       MENUSELECT_FUNCS        
         func_volume                                        MENUSELECT_FUNCS        
         func_evalexten                                     MENUSELECT_FUNCS        
         func_export                                        MENUSELECT_FUNCS        
         func_frame_drop                                    MENUSELECT_FUNCS        
         func_frame_trace                                   MENUSELECT_FUNCS        
         func_json                                          MENUSELECT_FUNCS        
         func_pitchshift                                    MENUSELECT_FUNCS        
         func_sayfiles                                      MENUSELECT_FUNCS        
         func_scramble                                      MENUSELECT_FUNCS        
         pbx_config                                         MENUSELECT_PBX          
         pbx_loopback                                       MENUSELECT_PBX          
         pbx_spool                                          MENUSELECT_PBX          
         pbx_ael                                            MENUSELECT_PBX          
         pbx_dundi                                          MENUSELECT_PBX          
         pbx_lua                                            MENUSELECT_PBX          
         pbx_realtime                                       MENUSELECT_PBX          
         res_aeap                                           MENUSELECT_RES          
         res_agi                                            MENUSELECT_RES          
         res_ari                                            MENUSELECT_RES          
         res_ari_applications                               MENUSELECT_RES          
         res_ari_asterisk                                   MENUSELECT_RES          
         res_ari_bridges                                    MENUSELECT_RES          
         res_ari_channels                                   MENUSELECT_RES          
         res_ari_device_states                              MENUSELECT_RES          
         res_ari_endpoints                                  MENUSELECT_RES          
         res_ari_events                                     MENUSELECT_RES          
         res_ari_mailboxes                                  MENUSELECT_RES          
         res_ari_model                                      MENUSELECT_RES          
         res_ari_playbacks                                  MENUSELECT_RES          
         res_ari_recordings                                 MENUSELECT_RES          
         res_ari_sounds                                     MENUSELECT_RES          
         res_clialiases                                     MENUSELECT_RES          
         res_clioriginate                                   MENUSELECT_RES          
         res_config_curl                                    MENUSELECT_RES          
         res_config_odbc                                    MENUSELECT_RES          
         res_config_sqlite3                                 MENUSELECT_RES          
         res_convert                                        MENUSELECT_RES          
         res_crypto                                         MENUSELECT_RES          
         res_curl                                           MENUSELECT_RES          
         res_fax                                            MENUSELECT_RES          
         res_format_attr_celt                               MENUSELECT_RES          
         res_format_attr_g729                               MENUSELECT_RES          
         res_format_attr_h263                               MENUSELECT_RES          
         res_format_attr_h264                               MENUSELECT_RES          
         res_format_attr_ilbc                               MENUSELECT_RES          
         res_format_attr_opus                               MENUSELECT_RES          
         res_format_attr_silk                               MENUSELECT_RES          
         res_format_attr_siren14                            MENUSELECT_RES          
         res_format_attr_siren7                             MENUSELECT_RES          
         res_format_attr_vp8                                MENUSELECT_RES          
         res_geolocation                                    MENUSELECT_RES          
         res_http_media_cache                               MENUSELECT_RES          
         res_http_post                                      MENUSELECT_RES          
         res_http_websocket                                 MENUSELECT_RES          
         res_limit                                          MENUSELECT_RES          
         res_manager_devicestate                            MENUSELECT_RES          
         res_manager_presencestate                          MENUSELECT_RES          
         res_musiconhold                                    MENUSELECT_RES          
         res_mutestream                                     MENUSELECT_RES          
         res_mwi_devstate                                   MENUSELECT_RES          
         res_mwi_external                                   MENUSELECT_RES          
         res_mwi_external_ami                               MENUSELECT_RES          
         res_odbc                                           MENUSELECT_RES          
         res_odbc_transaction                               MENUSELECT_RES          
         res_parking                                        MENUSELECT_RES          
         res_pjproject                                      MENUSELECT_RES          
         res_pjsip                                          MENUSELECT_RES          
         res_pjsip_acl                                      MENUSELECT_RES          
         res_pjsip_authenticator_digest MENUSELECT_RES                              
         res_pjsip_caller_id                                MENUSELECT_RES          
         res_pjsip_config_wizard                            MENUSELECT_RES          
         res_pjsip_dialog_info_body_gen MENUSELECT_RES                              
         res_pjsip_diversion                                MENUSELECT_RES          
         res_pjsip_dlg_options                              MENUSELECT_RES          
         res_pjsip_dtmf_info                                MENUSELECT_RES          
         res_pjsip_empty_info                               MENUSELECT_RES          
         res_pjsip_endpoint_identifier_ MENUSELECT_RES                              
         res_pjsip_endpoint_identifier_ MENUSELECT_RES                              
         res_pjsip_endpoint_identifier_ MENUSELECT_RES                              
         res_pjsip_exten_state                              MENUSELECT_RES          
         res_pjsip_geolocation                              MENUSELECT_RES          
         res_pjsip_header_funcs                             MENUSELECT_RES          
         res_pjsip_logger                                   MENUSELECT_RES          
         res_pjsip_messaging                                MENUSELECT_RES          
         res_pjsip_mwi                                      MENUSELECT_RES          
         res_pjsip_mwi_body_generator                       MENUSELECT_RES          
         res_pjsip_nat                                      MENUSELECT_RES          
         res_pjsip_notify                                   MENUSELECT_RES          
         res_pjsip_one_touch_record_inf MENUSELECT_RES                              
         res_pjsip_outbound_authenticat MENUSELECT_RES                              
         res_pjsip_outbound_publish                         MENUSELECT_RES          
         res_pjsip_outbound_registratio MENUSELECT_RES                              
         res_pjsip_path                                     MENUSELECT_RES          
         res_pjsip_pidf_body_generator                      MENUSELECT_RES          
         res_pjsip_pidf_digium_body_sup MENUSELECT_RES                              
         res_pjsip_pidf_eyebeam_body_su MENUSELECT_RES                              
         res_pjsip_publish_asterisk                         MENUSELECT_RES          
         res_pjsip_pubsub                                   MENUSELECT_RES          
         res_pjsip_refer                                    MENUSELECT_RES          
         res_pjsip_registrar                                MENUSELECT_RES          
         res_pjsip_rfc3326                                  MENUSELECT_RES          
         res_pjsip_rfc3329                                  MENUSELECT_RES          
         res_pjsip_sdp_rtp                                  MENUSELECT_RES          
         res_pjsip_send_to_voicemail                        MENUSELECT_RES          
         res_pjsip_session                                  MENUSELECT_RES          
         res_pjsip_sips_contact                             MENUSELECT_RES          
         res_pjsip_stir_shaken                              MENUSELECT_RES          
         res_pjsip_t38                                      MENUSELECT_RES          
         res_pjsip_transport_websocket                      MENUSELECT_RES          
         res_pjsip_xpidf_body_generator MENUSELECT_RES                              
         res_realtime                                       MENUSELECT_RES          
         res_resolver_unbound                               MENUSELECT_RES          
         res_rtp_asterisk                                   MENUSELECT_RES          
         res_rtp_multicast                                  MENUSELECT_RES          
         res_security_log                                   MENUSELECT_RES          
         res_sorcery_astdb                                  MENUSELECT_RES          
         res_sorcery_config                                 MENUSELECT_RES          
         res_sorcery_memory                                 MENUSELECT_RES          
         res_sorcery_memory_cache                           MENUSELECT_RES          
         res_sorcery_realtime                               MENUSELECT_RES          
         res_speech                                         MENUSELECT_RES          
         res_speech_aeap                                    MENUSELECT_RES          
         res_srtp                                           MENUSELECT_RES          
         res_stasis                                         MENUSELECT_RES          
         res_stasis_answer                                  MENUSELECT_RES          
         res_stasis_device_state                            MENUSELECT_RES          
         res_stasis_mailbox                                 MENUSELECT_RES          
         res_stasis_playback                                MENUSELECT_RES          
         res_stasis_recording                               MENUSELECT_RES          
         res_stasis_snoop                                   MENUSELECT_RES          
         res_stasis_test                                    MENUSELECT_RES          
         res_stir_shaken                                    MENUSELECT_RES          
         res_stun_monitor                                   MENUSELECT_RES          
         res_timing_dahdi                                   MENUSELECT_RES          
         res_timing_timerfd                                 MENUSELECT_RES          
         res_xmpp                                           MENUSELECT_RES          
         res_ael_share                                      MENUSELECT_RES          
         res_audiosocket                                    MENUSELECT_RES          
         res_calendar                                       MENUSELECT_RES          
         res_calendar_caldav                                MENUSELECT_RES          
         res_calendar_ews                                   MENUSELECT_RES          
         res_calendar_exchange                              MENUSELECT_RES          
         res_calendar_icalendar                             MENUSELECT_RES          
         res_chan_stats                                     MENUSELECT_RES          
         res_cliexec                                        MENUSELECT_RES          
         res_config_ldap                                    MENUSELECT_RES          
         res_config_pgsql                                   MENUSELECT_RES          
         res_corosync                                       MENUSELECT_RES          
         res_endpoint_stats                                 MENUSELECT_RES          
         res_fax_spandsp                                    MENUSELECT_RES          
         res_hep                                            MENUSELECT_RES          
         res_hep_pjsip                                      MENUSELECT_RES          
         res_hep_rtcp                                       MENUSELECT_RES          
         res_phoneprov                                      MENUSELECT_RES          
         res_pjsip_aoc                                      MENUSELECT_RES          
         res_pjsip_history                                  MENUSELECT_RES          
         res_pjsip_phoneprov_provider                       MENUSELECT_RES          
         res_pktccops                                       MENUSELECT_RES          
         res_prometheus                                     MENUSELECT_RES          
         res_remb_modifier                                  MENUSELECT_RES          
         res_smdi                                           MENUSELECT_RES          
         res_snmp                                           MENUSELECT_RES          
         res_statsd                                         MENUSELECT_RES          
         res_timing_kqueue                                  MENUSELECT_RES          
         res_timing_pthread                                 MENUSELECT_RES          
         res_tonedetect                                     MENUSELECT_RES          
         res_adsi                                           MENUSELECT_RES          
         res_config_sqlite                                  MENUSELECT_RES          
         res_monitor                                        MENUSELECT_RES          
         res_digium_phone                                   MENUSELECT_RES          
         test_abstract_jb                                   MENUSELECT_TESTS        
         test_acl                                           MENUSELECT_TESTS        
         test_aeap                                          MENUSELECT_TESTS        
         test_aeap_speech                                   MENUSELECT_TESTS        
         test_aeap_transaction                              MENUSELECT_TESTS        
         test_aeap_transport                                MENUSELECT_TESTS        
         test_amihooks                                      MENUSELECT_TESTS        
         test_aoc                                           MENUSELECT_TESTS        
         test_app                                           MENUSELECT_TESTS        
         test_ari                                           MENUSELECT_TESTS        
         test_ari_model                                     MENUSELECT_TESTS        
         test_ast_format_str_reduce                         MENUSELECT_TESTS        
         test_astobj2                                       MENUSELECT_TESTS        
         test_astobj2_thrash                                MENUSELECT_TESTS        
         test_astobj2_weaken                                MENUSELECT_TESTS        
         test_bridging                                      MENUSELECT_TESTS        
         test_bucket                                        MENUSELECT_TESTS        
         test_callerid                                      MENUSELECT_TESTS        
         test_capture                                       MENUSELECT_TESTS        
         test_cdr                                           MENUSELECT_TESTS        
         test_cel                                           MENUSELECT_TESTS        
         test_channel                                       MENUSELECT_TESTS        
         test_channel_feature_hooks                         MENUSELECT_TESTS        
         test_config                                        MENUSELECT_TESTS        
         test_conversions                                   MENUSELECT_TESTS        
         test_core_codec                                    MENUSELECT_TESTS        
         test_core_format                                   MENUSELECT_TESTS        
         test_crypto                                        MENUSELECT_TESTS        
         test_data_buffer                                   MENUSELECT_TESTS        
         test_db                                            MENUSELECT_TESTS        
         test_devicestate                                   MENUSELECT_TESTS        
         test_dlinklists                                    MENUSELECT_TESTS        
         test_dns                                           MENUSELECT_TESTS        
         test_dns_naptr                                     MENUSELECT_TESTS        
         test_dns_query_set                                 MENUSELECT_TESTS        
         test_dns_recurring                                 MENUSELECT_TESTS        
         test_dns_srv                                       MENUSELECT_TESTS        
         test_endpoints                                     MENUSELECT_TESTS        
         test_event                                         MENUSELECT_TESTS        
         test_expr                                          MENUSELECT_TESTS        
         test_file                                          MENUSELECT_TESTS        
         test_format_cache                                  MENUSELECT_TESTS        
         test_format_cap                                    MENUSELECT_TESTS        
         test_func_file                                     MENUSELECT_TESTS        
         test_gosub                                         MENUSELECT_TESTS        
         test_hashtab_thrash                                MENUSELECT_TESTS        
         test_heap                                          MENUSELECT_TESTS        
         test_http_media_cache                              MENUSELECT_TESTS        
         test_jitterbuf                                     MENUSELECT_TESTS        
         test_json                                          MENUSELECT_TESTS        
         test_linkedlists                                   MENUSELECT_TESTS        
         test_locale                                        MENUSELECT_TESTS        
         test_logger                                        MENUSELECT_TESTS        
         test_media_cache                                   MENUSELECT_TESTS        
         test_message                                       MENUSELECT_TESTS        
         test_mwi                                           MENUSELECT_TESTS        
         test_named_lock                                    MENUSELECT_TESTS        
         test_netsock2                                      MENUSELECT_TESTS        
         test_optional_api                                  MENUSELECT_TESTS        
         test_pbx                                           MENUSELECT_TESTS        
         test_poll                                          MENUSELECT_TESTS        
         test_res_pjsip_scheduler                           MENUSELECT_TESTS        
         test_res_pjsip_session_caps                        MENUSELECT_TESTS        
         test_res_rtp                                       MENUSELECT_TESTS        
         test_res_stasis                                    MENUSELECT_TESTS        
         test_sched                                         MENUSELECT_TESTS        
         test_scope_trace                                   MENUSELECT_TESTS        
         test_scoped_lock                                   MENUSELECT_TESTS        
         test_security_events                               MENUSELECT_TESTS        
         test_skel                                          MENUSELECT_TESTS        
         test_sorcery                                       MENUSELECT_TESTS        
         test_sorcery_astdb                                 MENUSELECT_TESTS        
         test_sorcery_memory_cache_thra MENUSELECT_TESTS                            
         test_sorcery_realtime                              MENUSELECT_TESTS        
         test_stasis                                        MENUSELECT_TESTS        
         test_stasis_channels                               MENUSELECT_TESTS        
         test_stasis_endpoints                              MENUSELECT_TESTS        
         test_stasis_state                                  MENUSELECT_TESTS        
         test_stream                                        MENUSELECT_TESTS        
         test_stringfields                                  MENUSELECT_TESTS        
         test_strings                                       MENUSELECT_TESTS        
         test_substitution                                  MENUSELECT_TESTS        
         test_taskprocessor                                 MENUSELECT_TESTS        
         test_threadpool                                    MENUSELECT_TESTS        
         test_time                                          MENUSELECT_TESTS        
         test_uri                                           MENUSELECT_TESTS        
         test_utils                                         MENUSELECT_TESTS        
         test_uuid                                          MENUSELECT_TESTS        
         test_vector                                        MENUSELECT_TESTS        
         test_voicemail_api                                 MENUSELECT_TESTS        
         test_websocket_client                              MENUSELECT_TESTS        
         test_xml_escape                                    MENUSELECT_TESTS        
         test_res_prometheus                                MENUSELECT_TESTS        
         DONT_OPTIMIZE                                      MENUSELECT_CFLAGS       
         COMPILE_DOUBLE                                     MENUSELECT_CFLAGS       
         DEBUG_THREADS                                      MENUSELECT_CFLAGS       
         DEBUG_FD_LEAKS                                     MENUSELECT_CFLAGS       
         BETTER_BACKTRACES                                  MENUSELECT_CFLAGS       
         LOTS_OF_SPANS                                      MENUSELECT_CFLAGS       
         MALLOC_DEBUG                                       MENUSELECT_CFLAGS       
         DEBUG_CHAOS                                        MENUSELECT_CFLAGS       
         BUILD_NATIVE                                       MENUSELECT_CFLAGS       
         ADD_CFLAGS_TO_BUILDOPTS_H                          MENUSELECT_CFLAGS       
         REF_DEBUG                                          MENUSELECT_CFLAGS       
         AO2_DEBUG                                          MENUSELECT_CFLAGS       
         REBUILD_PARSERS                                    MENUSELECT_CFLAGS       
         LOW_MEMORY                                         MENUSELECT_CFLAGS       
         DISABLE_INLINE                                     MENUSELECT_CFLAGS       
         OPTIONAL_API                                       MENUSELECT_CFLAGS       
         USE_HOARD_ALLOCATOR                                MENUSELECT_CFLAGS       
         RADIO_RELAX                                        MENUSELECT_CFLAGS       
         G711_NEW_ALGORITHM                                 MENUSELECT_CFLAGS       
         G711_REDUCED_BRANCHING                             MENUSELECT_CFLAGS       
         TEST_CODING_TABLES                                 MENUSELECT_CFLAGS       
         TEST_TANDEM_TRANSCODING                            MENUSELECT_CFLAGS       
         ADDRESS_SANITIZER                                  MENUSELECT_CFLAGS       
         THREAD_SANITIZER                                   MENUSELECT_CFLAGS       
         LEAK_SANITIZER                                     MENUSELECT_CFLAGS       
         UNDEFINED_SANITIZER                                MENUSELECT_CFLAGS       
         BUSYDETECT_TONEONLY                                MENUSELECT_CFLAGS       
         BUSYDETECT_COMPARE_TONE_AND_SI MENUSELECT_CFLAGS                           
         BUSYDETECT_DEBUG                                   MENUSELECT_CFLAGS       
         INTEGER_CALLERID                                   MENUSELECT_CFLAGS       
         astcanary                                          MENUSELECT_UTILS        
         astdb2sqlite3                                      MENUSELECT_UTILS        
         astdb2bdb                                          MENUSELECT_UTILS        
         check_expr                                         MENUSELECT_UTILS        
         check_expr2                                        MENUSELECT_UTILS        
         smsq                                               MENUSELECT_UTILS        
         stereorize                                         MENUSELECT_UTILS        
         streamplayer                                       MENUSELECT_UTILS        
         conf_bridge_binaural_hrir_impo MENUSELECT_UTILS                            
         aelparse                                           MENUSELECT_UTILS        
         astman                                             MENUSELECT_UTILS        
         conf2ael                                           MENUSELECT_UTILS        
         muted                                              MENUSELECT_UTILS        
         agiest.agi                                         MENUSELECT_AGIS         
         eagiest                                            MENUSELECT_AGIS         
         eagiphinxest                                       MENUSELECT_AGIS         
         jukebox.agi                                        MENUSELECT_AGIS         
         COREOUNDSNAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSNLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSNLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSNSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSN729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSN722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSNLN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSNIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSNIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AUAV                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AULAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AULAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AUSM                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AU729                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AU722                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AULN16                                  MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AUIREN7                                 MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_AUIREN14                                MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBAV                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBLAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBLAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBSM                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GB729                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GB722                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBLN16                                  MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBIREN7                                 MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_GBIREN14                                MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZAV                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZLAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZLAW                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZSM                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZ729                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZ722                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZLN16                                  MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZIREN7                                 MENUSELECT_CORE_SOUNDS  
         COREOUNDSN_NZIREN14                                MENUSELECT_CORE_SOUNDS  
         COREOUNDSSAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSSLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSSLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSSSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSS729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSS722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSSLN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSSIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSSIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSRAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSRLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSRLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSRSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSR729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSR722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSRLN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSRIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSRIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSTAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSTLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSTLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSTSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDST729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDST722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSTLN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSTIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSTIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSUAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSULAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSULAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSUSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSU729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSU722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSULN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSUIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSUIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSAAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSALAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSALAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSASM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSA729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSA722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSALN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSAIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSAIREN14                                   MENUSELECT_CORE_SOUNDS  
         COREOUNDSVAV                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSVLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSVLAW                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSVSM                                       MENUSELECT_CORE_SOUNDS  
         COREOUNDSV729                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSV722                                      MENUSELECT_CORE_SOUNDS  
         COREOUNDSVLN16                                     MENUSELECT_CORE_SOUNDS  
         COREOUNDSVIREN7                                    MENUSELECT_CORE_SOUNDS  
         COREOUNDSVIREN14                                   MENUSELECT_CORE_SOUNDS  
         MOHPSOUNDAV                                        MENUSELECT_MOH          
         MOHPSOUNDLAW                                       MENUSELECT_MOH          
         MOHPSOUNDLAW                                       MENUSELECT_MOH          
         MOHPSOUNDSM                                        MENUSELECT_MOH          
         MOHPSOUND729                                       MENUSELECT_MOH          
         MOHPSOUND722                                       MENUSELECT_MOH          
         MOHPSOUNDLN16                                      MENUSELECT_MOH          
         MOHPSOUNDIREN7                                     MENUSELECT_MOH          
         MOHPSOUNDIREN14                                    MENUSELECT_MOH          
         EXTRAOUNDSNAV                                      MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNLAW                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNLAW                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNSM                                      MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN729                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN722                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNLN16                                    MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNIREN7                                   MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSNIREN14                                  MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBAV                                   MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBLAW                                  MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBLAW                                  MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBSM                                   MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GB729                                  MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GB722                                  MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBLN16                                 MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBIREN7                                MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSN_GBIREN14                               MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRAV                                      MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRLAW                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRLAW                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRSM                                      MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSR729                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSR722                                     MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRLN16                                    MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRIREN7                                   MENUSELECT_EXTRA_SOUNDS 
         EXTRAOUNDSRIREN14                                  MENUSELECT_EXTRA_SOUNDS 


6. List options within the category `MENUSELECT_AGIS`:
   ```
   menuselect/menuselect --list-category MENUSELECT_AGIS
   ```
   
   ### EXAMPLE OUTPUT: 
     - agi-test.agi
     - eagi-test
     - eagi-sphinx-test
     - jukebox.agi

7. List all available categories:
   ```
   menuselect/menuselect --category-list
   ```
   
   OUTPUT:
            MENUSELECT_ADDONS
            MENUSELECT_APPS
            MENUSELECT_BRIDGES
            MENUSELECT_CDR
            MENUSELECT_CEL
            MENUSELECT_CHANNELS
            MENUSELECT_CODECS
            MENUSELECT_FORMATS
            MENUSELECT_FUNCS
            MENUSELECT_PBX
            MENUSELECT_RES
            MENUSELECT_TESTS
            MENUSELECT_CFLAGS 
            MENUSELECT_UTILS
            MENUSELECT_AGIS
            MENUSELECT_CORE_SOUNDS
            MENUSELECT_MOH
            MENUSELECT_EXTRA_SOUNDS

8. Display usage information:
   ```
   menuselect/menuselect --help
   ```
   ### USAGE: 
    ```
    Usage: menuselect/menuselect [--enable <option>] [--disable <option>]
       [--enable-category <category>] [--enable-all]
       [--disable-category <category>] [--disable-all] [...]
       [<config-file> [...]]
    Usage: menuselect/menuselect { --check-deps | --list-options
       | --list-category <category> | --category-list | --help }
       [<config-file> [...]]
    ```

**Note:** Replace `<option>` and `<category>` with the actual names of the configuration options and categories.

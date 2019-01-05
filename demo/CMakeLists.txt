project(waveform)
set(COMMON_SOURCE_FILES ../Blip_Buffer.h ../Blip_Buffer.cpp ../player/player.cpp ../player/Wave_Writer.cpp)
add_executable(waveform 1.waveform.cpp ${COMMON_SOURCE_FILES})

project(square)
add_executable(square 2.square.cpp ${COMMON_SOURCE_FILES})

project(clock_rate)
add_executable(clock_rate 3.clock_rate.cpp ${COMMON_SOURCE_FILES})

project(continuous)
add_executable(continuous 4.continuous.cpp ${COMMON_SOURCE_FILES})

project(buffering)
add_executable(buffering buffering.cpp ${COMMON_SOURCE_FILES})

project(delta_synth)
add_executable(delta_synth delta_synth.cpp ${COMMON_SOURCE_FILES})

project(external_mixing)
add_executable(external_mixing external_mixing.cpp ${COMMON_SOURCE_FILES})

project(multiple_waves)
add_executable(multiple_waves multiple_waves.cpp ${COMMON_SOURCE_FILES})

project(sample_formats)
add_executable(sample_formats sample_formats.cpp ../Blip_Buffer.h ../Blip_Buffer.cpp ../player/Wave_Writer.cpp )

project(sdl_audio)
add_executable(sdl_audio sdl_audio.cpp ../Blip_Buffer.h ../Blip_Buffer.cpp ../player/Wave_Writer.cpp ../sdl_player/Audio_Scope.cpp ../sdl_player/Sync_Audio.cpp)
target_link_libraries(sdl_audio SDL)

project(stereo)
add_executable(stereo stereo.cpp ${COMMON_SOURCE_FILES})

project(treble_bass)
add_executable(treble_bass treble_bass.cpp ${COMMON_SOURCE_FILES})
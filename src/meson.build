project('staffing-tools-project-manual', version : '1.0')

gem = find_program('gem')
asciidoctor = find_program('asciidoctor')

run_command(gem, 'which', 'asciidoctor-pdf', check:true)
message('gem asciidoctor-pdf was found')

chapters = files(
    'chapters/SUMMARY.adoc',
    'chapters/DEFINITIONS.adoc',
    'chapters/GOALS.adoc',
    'chapters/PERSONAS.adoc',
    'chapters/USER_STORIES.adoc'
)

custom_target(
    'manual-pdf',
    depend_files : chapters,
    input : 'PROJECT_MANUAL.adoc',
    command : [asciidoctor, '-r', 'asciidoctor-pdf', '-b', 'pdf', '-o', 'project_manual.pdf', '@INPUT@'],
    output : 'project_manual.pdf',
    build_by_default : true
)

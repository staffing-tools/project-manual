project('staffing-tools-project-manual', version : '1.0')

chapters = files(
    'chapters/DEFINITIONS.adoc',
    'chapters/GOALS.adoc',
    'chapters/PERSONAS.adoc',
    'chapters/USER_STORIES.adoc'
)

custom_target(
    'manual-pdf',
    depend_files : chapters,
    input : 'PROJECT_MANUAL.adoc',
    command : ['asciidoctor', '-rasciidoctor-pdf', '-b', 'pdf', '-o', 'project_manual.pdf', '@INPUT@'],
    output : 'project_manual.pdf',
    build_by_default : true
)

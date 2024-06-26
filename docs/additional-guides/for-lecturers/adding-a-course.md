You are invited to design your own course for AI-LAB. You can create your own pages within the documentation and upload course materials directly to the AI-LAB server.

## How to add a course to the documentation
To include a course in the AI-LAB documentation, use [Markdown](https://en.wikipedia.org/wiki/Markdown) format and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) for styling. Follow these steps to create a new course:

1. Start by forking the repository to your GitHub account from here: [https://github.com/aau-claaudia/ailab-docs/fork](https://github.com/aau-claaudia/ailab-docs/fork).
2. In the `/docs/courses` directory, create a new folder named after your course. This folder will contain your `.md` files, which form the basis of your course content.
      * For design tips, refer to our [page design guide](/additional-guides/for-lecturers/page-design-guide).
      * To preview your page, install Material for MkDocs by following this [getting started guide](https://squidfunk.github.io/mkdocs-material/getting-started/).
      * Your course series may include multiple files, e.g., `tensorflow-course-1.md`, `tensorflow-course-2.md`, etc.
3. Once you have made the necessary changes, submit a pull request to the main repository.
4. We will review your changes and, if everything is in order, merge your pull request.

## Adding container image files to AI-LAB
You can add your own container image files to the `/ceph/container` directory on AI-LAB. Simply `cp` the container from your own directory to the `/ceph/container` or use `scp` if you want to transfer it from your local computer. Take a look at [File management](/getting-started/file-management) for more details. 

We also have guides on how to [download container images](/additional-guides/download-images-from-ngc) and how to [build your own container image](/additional-guides/building-your-own-container-image).


## Adding course material to AI-LAB
Similar to adding container image files, you can add files to the `/ceph/course` directory on AI-LAB. It could be datasets or scripts, but also container images. Please make a directory (`mkdir [name]`) that you can store your files in.
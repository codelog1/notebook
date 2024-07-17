---
layout: post
title: Jekyll Now 블로그에 이미지 삽입하는 방법
categories: [Jekyll Now, 블로그, 깃허브]
tags: [이미지, READNE, 구글 드라이브]
---


# Jekyll Now 블로그에 이미지 삽입하는 방법

Jekyll Now 블로그에 이미지를 삽입하는 방법은 여러 가지가 있으며, 다음은 대표적인 방법들입니다:

### 1. GitHub 저장소에 이미지 업로드하기

이미지를 GitHub 저장소에 업로드하고 해당 이미지를 마크다운 문법을 이용해 삽입할 수 있습니다.

1.  **이미지 업로드**: 깃허브 개인 저장소에 이미지를 업로드합니다. 예를 들어, `assets/images` 디렉토리에 이미지를 업로드합니다.
    
2.  **마크다운 문법 사용**: 이미지 경로를 마크다운 문법으로 삽입합니다.
    
    ```markdown
    ![이미지 설명](/assets/images/이미지이름.jpg)
    
    ```
    

### 2. 외부 이미지 링크 사용하기

외부 이미지를 링크로 삽입하는 방법입니다.

1.  **이미지 링크 확보**: 외부 이미지를 직접 링크로 확보합니다.
    
2.  **삽입**: 링크를 마크다운으로 삽입합니다.
    
    ```markdown
    ![이미지 설명](<http://example.com/이미지이름.jpg>)
    
    ```
    

### 3. GitHub 사용자 콘텐츠 이용하기

GitHub 사용자 콘텐츠 링크를 사용하여 이미지를 삽입할 수 있습니다. 예를 들어, GitHub에서 제공하는 `raw` 링크를 사용할 수 있습니다.

1.  **이미지 업로드**: 이미지를 자신의 GitHub 리포지토리에 업로드합니다.
    
2.  **raw 링크 생성**: raw 콘텐츠 URL을 사용해 링크를 생성합니다.
    
    ```markdown
    ![이미지 설명](<https://raw.githubusercontent.com/사용자명/레포지토리명/브랜치명/경로/이미지이름.jpg>)
    
    ```
    

### 4. Jekyll 플러그인 이용하기

특정 Jekyll 플러그인을 이용해 이미지를 쉽게 삽입할 수도 있습니다.

1.  **Jekyll 플러그인 설치**: `jekyll-assets` 같은 플러그인을 설치합니다.
    
2.  **이미지 삽입**: 플러그인의 마크다운 태그를 사용해 이미지를 삽입합니다.
    
    ```
    {% asset_path images/image.jpg %}
    
    ```
    

### 추가 팁

-   이미지를 삽입하는 문장 뒤에 크기 등을 조절할 수 있도록 추가적인 속성을 선언할 수 있습니다.
    
    ```markdown
    ![이미지 설명](/assets/images/이미지이름.jpg){: width="600" height="400"}
    
    ```
    

이와 같은 방법들을 통해 Jekyll 블로그에 이미지를 효과적으로 삽입할 수 있습니다.

🔗 [[Blog] GitHub Pages 블로그 이미지 업로드](https://hyeonjiwon.github.io/blog/markdown_img/)

🔗 [자바스크립트 라이브러리 배포를 위한 웹팩(webpack) 설정 경험기](https://blog.hyeyoonjung.com/2019/05/26/setting-webpack-for-javascript-library/)

----------

# **Github 블로그 이미지 업로드 방법**

GitHub 블로그에 이미지를 업로드하는 방법은 여러 가지가 있습니다. 아래에 몇 가지 대표적인 방법을 정리했습니다.

### 1. Issues를 이용한 이미지 업로드

이 방법은 가장 간단하고 널리 사용됩니다.

1.  GitHub 리포지토리에 접속합니다.
2.  "Issues" 탭으로 이동하여 "New issue" 버튼을 클릭합니다.
3.  텍스트 박스에 이미지를 드래그 앤 드롭하거나 붙여넣습니다.
4.  이미지가 업로드되면 생성된 Markdown 코드를 복사합니다.
5.  이 코드를 원하는 위치에 붙여넣으면 됩니다.

예시:

```markdown
![image](<https://user-images.githubusercontent.com/username/repo/image.png>)

```

이 방법을 사용하면 GitHub가 자동으로 이미지를 처리하고 URL을 생성해줍니다.

🔗 [[Blog] GitHub Pages 블로그 이미지 업로드](https://hyeonjiwon.github.io/blog/markdown_img/)

🔗 [[블로그] github에 이미지 저장 없이 업로드하기](https://cultivo-hy.github.io/blog/github/tip/2019/03/11/%EC%9D%B4%EB%AF%B8%EC%A7%80-%EC%97%85%EB%A1%9C%EB%93%9C/)

### 2. 로컬 저장소를 통한 이미지 업로드

1.  로컬 저장소에서 블로그 프로젝트 폴더로 이동합니다.
2.  'img' 폴더를 만들고 업로드할 이미지 파일을 이 폴더에 저장합니다.
3.  Markdown 파일에서 이미지 파일의 경로를 지정합니다.

예시:

```markdown
![image](./img/your-image.png)

```

이 방법은 이미지 파일이 로컬 저장소와 함께 관리되며, 직접 경로를 설정해줄 수 있습니다.

🔗 [Github 블로그 image 삽입하기](https://velog.io/@uzchu/Github-%EB%B8%94%EB%A1%9C%EA%B7%B8-image-%EC%82%BD%EC%9E%85%ED%95%98%EA%B8%B0)

### 3. 외부 호스팅 서비스 이용

Google Drive, Dropbox, One Drive 등의 외부 호스팅 서비스를 이용하여 이미지를 업로드하고 URL을 가져올 수 있습니다.

1.  이미지를 외부 호스팅 서비스에 업로드합니다.
2.  해당 이미지의 공유 가능한 URL을 복사합니다.
3.  Markdown 파일에 URL을 삽입합니다.

예시:

```markdown
![image](<https://drive.google.com/your-image-url>)

```

이 방법은 외부 호스팅 서비스의 장점을 활용하여 이미지를 관리할 수 있습니다.

🔗 [깃허브(GitHub, jekyll) 블로그 이미지 호스팅 하기 (원드라이브, 구글드라이브)](https://pioneergu.github.io/posts/jekyll-github-blog-image-hosting/)

### 4. GitHub Pages에 직접 이미지 파일 업로드

1.  GitHub 웹사이트에서 리포지토리의 `/docs/assets` 디렉토리로 이동합니다.
2.  "Add file" 버튼을 클릭하고 이미지를 업로드합니다.
3.  이미지를 업로드한 후 Markdown 파일에 해당 이미지의 경로를 지정합니다.

예시:

```markdown
![image](/docs/assets/your-image.png)

```

이 방법은 GitHub Pages의 구조 내에서 이미지를 관리하는 데 유용합니다.

🔗 [Github 블로그에 이미지 넣기](https://seong6496.tistory.com/311)

이들 방법을 통해 GitHub 블로그에 쉽게 이미지를 업로드하고 사용할 수 있습니다. 각각의 방법은 상황에 따라 적절히 선택하시면 됩니다.

----------

# **깃허브 페이지에 이미지 올리는 방법**

GitHub Pages에 이미지를 올리는 방법에는 여러 가지가 있습니다. 아래에 일부 방법을 정리하였습니다.

### 방법 1: 직접 저장소에 업로드

1.  **이미지 파일 준비**: 사용하려는 이미지를 준비합니다.
    
2.  **저장소 이동**: 깃헙 페이지의 저장소로 이동합니다.
    
3.  **파일 업로드**: `Add file` 버튼을 클릭하고 `Upload files`를 이용하여 이미지를 업로드합니다.
    
    🔗 [The Least You Need to Know About GitHub Pages](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html)
    
    🔗 [Adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
    

### 방법 2: Issues 탭 이용

1.  **Issues 탭으로 이동**: 저장소 상단의 `Issues` 탭으로 이동합니다.
    
2.  **New Issue 생성**: 오른쪽 상단의 `New issue` 버튼을 클릭하여 새 이슈를 생성합니다.
    
3.  **이미지 업로드**: 생성된 이슈의 텍스트 박스로 이미지를 드래그하거나 복사해서 붙여넣기 합니다. 업로드가 완료되면 이미지 URL을 복사할 수 있습니다.
    
    🔗 [GitHub Pages 블로그 이미지 업로드](https://hyeonjiwon.github.io/blog/markdown_img/)
    
    🔗 [깃허브 README.md에 이미지 올리기 (feat.Issue)](https://aiday.tistory.com/83)
    
    🔗 [깃허브 readme에 이미지 올리는 방법](https://coding-with-jina.tistory.com/165)
    
    🔗 [Upload Images to GitHub's Content Delivery Network](https://gist.github.com/NawalJAhmed/2168f7659c08b6a033e7f6daf8db69a6)
    

### 방법 3: HTML img 태그를 사용

GitHub Pages는 GitHub-flavored Markdown(GFM)을 지원하므로, HTML 태그를 사용할 수 있습니다.

1.  **이미지 URL 복사**: 업로드된 이미지의 URL을 복사합니다.
    
2.  **HTML img 태그 사용**: 아래의 형식으로 Markdown 파일에 이미지 태그를 작성합니다.
    
    ```markdown
    <img src="이미지_URL" alt="Image Description" />
    
    ```
    

이를 통해 이미지가 GitHub Pages에서 렌더링 됩니다.

🔗 [how to insert a photo into github-pages!?](https://github.com/orgs/community/discussions/52434)

🔗 [how to insert a photo into github-pages!?](https://www.reddit.com/r/github/comments/12hgkfw/how_to_insert_a_photo_into_githubpages/)

### 방법 4: 외부 CDN 이용

GitHub Pages에 이미지를 효과적으로 호스팅하기 위해 jsDelivr와 같은 CDN을 사용할 수 있습니다.

1.  **이미지 업로드**: 이미지 파일을 저장소에 업로드합니다.
    
2.  **jsDelivr URL 생성**: 업로드한 파일의 URL에 `https://cdn.jsdelivr.net/gh/`를 사용하여 CDN URL을 생성합니다.
    
🔗 [깃허브(GitHub, jekyll) 블로그 이미지 호스팅 하기 (원드라이브, 구글드라이브)](https://pioneergu.github.io/posts/jekyll-github-blog-image-hosting/)
    

이와 같은 방법들을 통해 GitHub Pages에 이미지를 손쉽게 업로드하고 사용할 수 있습니다.

----------

# **깃허브 README.md에 이미지 추가하기**

깃허브 [README.md](http://readme.md/) 파일에 이미지를 추가하는 방법은 여러 가지가 있습니다. 아래 다양한 방법을 소개합니다.

### 방법 1: Issue 활용하기

1.  **Issue 탭 열기**: 프로젝트의 Issue 탭으로 이동합니다.
    
2.  **새 Issue 작성**: "New Issue" 버튼을 눌러 새 이슈 작성 화면으로 들어갑니다.
    
3.  **이미지 업로드**: 내용 입력 칸에 이미지를 드래그 앤 드롭하거나 파일 선택 기능을 활용하여 이미지를 업로드합니다.
    
4.  **이미지 주소 복사**: 업로드된 이미지의 URL 주소를 복사합니다.
    
5.  **README.md에 추가**: [README.md](http://readme.md/) 파일에 다음과 같은 형식으로 이미지 URL을 삽입합니다.
    
    ```markdown
    ![이미지 설명](이미지 URL)
    
    ```
    

	예:

	```markdown
	![로고](<https://github.com/사용자명/저장소명/issues/1#issue-이미지ID>)

	```


🔗 [Github Readme에 이미지 올리기](https://worthpreading.tistory.com/83)

🔗 [GitHub - Image 올리기 (README, Issue, PR)](https://caileb.tistory.com/201)

### 방법 2: 외부 호스팅 없이 이미지 추가

외부 호스팅을 사용하지 않고 GitHub 자체의 기능을 활용해 이미지를 추가할 수도 있습니다.

1.  **이미지 Base64 인코딩**: 이미지를 Base64로 인코딩합니다. 온라인 인코더를 사용하면 쉽게 인코딩할 수 있습니다.
    
2.  **코드 추가**: 인코딩된 이미지를 [README.md](http://readme.md/) 파일에 직접 추가합니다.
    
    ```markdown
    <img src="data:image/png;base64,이미지 데이터" alt="이미지 설명" />
    
    ```
    

또는 GitHub의 원시 URL 기능을 사용할 수도 있습니다.

1.  **이미지 파일 업로드**: 이미지 파일을 저장소의 원하는 위치에 업로드합니다.
    
2.  **원시 URL 사용**: 이미지 파일의 파일 브라우저에서 "Raw" 버튼을 누르고 복사한 URL을 사용합니다.
    
    ```markdown
    ![이미지 설명](<https://raw.githubusercontent.com/사용자명/저장소명/브랜치명/경로/파일명>)
    
    ```
    


🔗 [외부 호스팅 없이 GitHub README.md에 이미지 추가하기](https://www.tempmail.us.com/ko/python/%EC%99%B8%EB%B6%80-%ED%98%B8%EC%8A%A4%ED%8C%85-%EC%97%86%EC%9D%B4-github-readme-md%EC%97%90-%EC%9D%B4%EB%AF%B8%EC%A7%80-%EC%B6%94%EA%B0%80%ED%95%98%EA%B8%B0)

### 방법 3: 저장소에 이미지 파일 추가

1.  **img 폴더 생성**: 프로젝트 루트 또는 원하는 경로에 `img` 폴더를 생성합니다.
    
2.  **이미지 파일 업로드**: `img` 폴더 안에 이미지 파일을 업로드합니다.
    
3.  **URL 참고**: 이미지 파일의 경로를 참조하여 [README.md](http://readme.md/) 파일에 이미지 링크를 추가합니다.
    
    ```markdown
    ![이미지 설명](img/파일명.png)
    
    ```
    


🔗 [[깃허브] README.md에 이미지 추가하는 방법](https://jeonge.tistory.com/66)

🔗 [36 깃(Git) - 깃허브 리드미(README) 3 : 이미지 삽입하기](https://abled.tistory.com/40)

### 방법 4: Drag & Drop 사용

1.  **[readme.md](http://readme.md/) 파일 편집**: GitHub 웹 인터페이스에서 [README.md](http://readme.md/) 파일을 편집합니다.
    
2.  **이미지 드롭**: 편집 화면에서 내용을 작성하면서 드래그 앤 드롭으로 이미지를 추가합니다.
    
3.  **이미지 URL 복사**: 이미지의 URL을 복사하여 적절한 위치에 삽입합니다.
    
    ```markdown
    ![이미지 설명](이미지 URL)
    
    ```
    

참조: 

🔗 [Readme 파일에 이미지 넣기 (마크다운 이미지)](https://cutemoomin.tistory.com/entry/Readme-%ED%8C%8C%EC%9D%BC%EC%97%90-%EC%9D%B4%EB%AF%B8%EC%A7%80-%EB%84%A3%EA%B8%B0-%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%EC%9D%B4%EB%AF%B8%EC%A7%80)

🔗 [[Github] README.md에 Image 넣기 & Image Size 조절하기](https://bugloss-chestnut.tistory.com/37)

각 방법은 상황에 따라 편한 방법을 선택해 사용하면 됩니다. 참고한 자료에서 구체적인 과정과 예제를 제공하므로, 필요에 따라 참조하면 도움이 될 것입니다.

----------

# **Jekyll Now 블로그 마크다운 이미지 추가**

Jekyll Now 블로그에 마크다운을 사용하여 이미지를 추가하는 방법은 다음과 같습니다:

### 1. 이미지 파일 준비

먼저 GitHub 저장소에 업로드하려는 이미지를 준비합니다. 보통 이미지 파일은 `/assets/images` 디렉토리에 넣는 것이 일반적입니다.

### 2. 이미지 업로드

이미지를 저장소에 업로드합니다. 이를 위해 GitHub 웹 인터페이스를 사용하거나 로컬 저장소에 직접 이미지를 추가한 후 커밋하고 푸시할 수 있습니다.

**GitHub 웹 인터페이스를 이용한 업로드**

1.  저장소에서 `assets/images` 디렉토리로 이동합니다.
2.  “Add file” 버튼을 클릭하고 "Upload files"를 선택합니다.
3.  업로드할 이미지 파일을 선택합니다.
4.  파일 업로드를 완료한 후 커밋 메시지를 작성하고 "Commit changes" 버튼을 클릭합니다.

### 3. 마크다운 파일에 이미지 삽입

업로드한 이미지를 마크다운 파일에서 사용하는 방법은 다음과 같습니다:

```markdown
![이미지 설명](이미지 경로)

```

예를 들어, `assets/images/example.png`라는 파일을 업로드한 경우, 마크다운 파일 내에서 다음과 같이 이미지를 삽입할 수 있습니다:

```markdown
![Example Image](/assets/images/example.png)

```

이렇게 하면 블로그 포스트에 해당 이미지가 표시됩니다.

### 4. 이미지 경로 확인

경로가 정확하지 않을 경우 이미지가 표시되지 않으므로 경로를 다시 확인합니다. 이미지 경로는 대소문자를 정확히 구분해야 합니다.

더 자세한 예제와 설명은 다음 참고 링크를 통해 확인할 수 있습니다:

    
🔗 [[Blog] GitHub Pages 블로그 이미지 업로드](https://hyeonjiwon.github.io/blog/markdown_img/)

🔗 [마크다운(Markdown) 문법(Syntax) 2](https://jeongseon-lee.github.io/posts/markdown-syntax2/)

----------

# **Jekyll Now 블로그 글에 구글 드라이브 이미지 삽입하는 방법**

Jekyll Now 블로그에 구글 드라이브 이미지를 삽입하는 방법은 일반적으로 다음과 같은 단계를 따릅니다:

### **1. 구글 드라이브에 이미지 업로드**:

-   먼저 구글 드라이브에 삽입할 이미지를 업로드합니다.

### **2. 이미지 공유 설정 변경**:

-   업로드된 이미지에서 오른쪽 버튼을 클릭하고 "공유"를 선택합니다.
-   "링크가 있는 모든 사용자에게 공개"로 설정한 뒤 제공된 링크를 복사합니다.

### **3. 공유 링크를 이미지 URL로 변환**:

-   구글 드라이브 링크의 기본 형식은 `https://drive.google.com/file/d/FILE_ID/view?usp=sharing` 입니다.
-   이를 다음과 같은 형식으로 변경해야 합니다: `https://drive.google.com/uc?export=view&id=FILE_ID`.
-   여기서 `FILE_ID`는 구글 드라이브 링크에서 파일 ID 부분을 의미합니다.

### **4. Jekyll Markdown에 이미지 삽입**:

-   변환한 이미지 URL을 Jekyll Markdown 양식에 맞춰 사용합니다. 예를 들어:
    
    ```markdown
    ![설명 텍스트](<https://drive.google.com/uc?export=view&id=FILE_ID>)
    
    ```
    

### 참고할 만한 자료들:

-   사용자들은 구글 드라이브의 이미지를 삽입하기 위해 링크 변환 절차를 밟아야 함을 명시하고 있습니다.
    
🔗 [[Jekyll Blog] 마크다운(Markdown) 사용법 및 예제](https://theorydb.github.io/envops/2019/05/22/envops-blog-how-to-use-md/)
    
🔗 [Making Websites for Fun and Spite](https://daniellethurow.com/blog/2020/12/7/making-websites-for-fun-and-spite)
    
-   문제가 발생할 경우, GitHub 페이지에서 지원하는 형식을 확인하거나 `.nojekyll` 파일을 추가해 Jekyll의 기본 설정을 무시할 수 있습니다.
    
🔗 [Images not displaying in Github Pages?](https://stackoverflow.com/questions/41468951/images-not-displaying-in-github-pages)
    

이 단계를 따라하면 Jekyll Now 블로그에 구글 드라이브 이미지를 성공적으로 삽입할 수 있습니다.

----------

# Jekyll Now 블로그 글에 구글 드라이브 이미지 삽입할 때 이미지 크기 설정 방법

Jekyll Now 블로그에 구글 드라이브 이미지를 삽입하면서 이미지 크기를 설정하는 방법은 다음과 같습니다. 여기에 구글 드라이브 이미지의 공유 링크를 사용하고, HTML과 CSS를 조합하여 이미지 크기를 조절할 수 있습니다.

### 1. 구글 드라이브 이미지 공유 링크 생성

먼저 구글 드라이브에서 이미지를 공유하기 위해 아래 단계를 따릅니다:

1.  구글 드라이브에서 이미지를 찾습니다.
2.  이미지 파일을 우클릭하고 "공유" 옵션을 선택합니다.
3.  "링크로 공유"를 활성화한 다음 "링크 복사"를 클릭합니다.

### 2. Jekyll Now 블로그 포스트에 이미지 삽입

이제 Jekyll Now 블로그 포스트에 이미지를 삽입합니다. 복사한 구글 드라이브 링크를 사용하여 아래와 같이 이미지를 추가합니다:

```markdown
![Alt text](<https://drive.google.com/uc?export=view&id=드라이브파일ID>)

```

여기서 `드라이브파일ID`는 링크에서 추출한 파일 ID입니다.

### 3. 이미지 크기 설정

이미지 크기를 조절하려면 HTML 태그를 사용하여 이미지의 너비(width)나 높이(height)를 설정할 수 있습니다. 예를 들어, 다음 예시는 이미지 너비를 300 픽셀로 설정합니다:

```html
<img src="<https://drive.google.com/uc?export=view&id=드라이브파일ID>" width="300" alt="Alternative text">

```

이와 같이 마크다운 파일 내에 HTML 태그를 사용할 수 있습니다.

### 예제

아래는 전체 예시입니다:

```markdown
---
layout: post
title: "구글 드라이브 이미지 삽입 예제"
---

이미지 예시:

<img src="<https://drive.google.com/uc?export=view&id=드라이브파일ID>" width="300" alt="구글 드라이브 이미지">

```

위의 방법을 사용하면 Jekyll Now 블로그 글에 구글 드라이브 이미지를 삽입하고 크기를 설정할 수 있습니다. 추가로 다양한 CSS 스타일을 적용할 수도 있습니다.

추가 정보는 관련 블로그를 참고하세요.

🔗 [app.md](https://github.com/hyunjun/bookmarks/blob/master/app.md)  ⇒ autohotkey bookmarks

----------

# **Jekyll Now 블로그에 이미지 삽입하면서 이미지 크기 설정하는 방법**

Jekyll Now 블로그에 이미지를 삽입하면서 이미지 크기를 설정하는 방법은 여러 가지가 있습니다. 아래와 같은 방법을 사용할 수 있습니다.

### 1. HTML 태그 사용

Markdown에서 HTML 태그를 직접 사용하여 이미지를 삽입하고 크기를 조절할 수 있습니다. 예를 들어:

```html
<img src="image.jpg" alt="sample image" width="300" height="200" />

```

위의 코드에서는 `width`와 `height` 속성을 사용하여 이미지의 크기를 조절할 수 있습니다.

🔗 [image resize in github flavored markdown.](https://gist.github.com/uupaa/f77d2bcf4dc7a294d109)

### 2. 스타일 속성 사용

Markdown에서 스타일 속성을 사용하여 크기를 조절할 수도 있습니다. 예를 들어:

```html
<img src="image.jpg" alt="sample image" style="width:300px; height:200px;"/>

```

이 방법 또한 HTML을 사용하여 이미지를 삽입하는 방식입니다.

🔗 [How to set size/rotate image in jekyll?](https://stackoverflow.com/questions/53992317/how-to-set-size-rotate-image-in-jekyll)

🔗 [Hydejack Post Writing Tips & Tricks](https://lazyren.github.io/devlog/hydejack-post-writing-tips-tricks.html)

### 3. Jekyll Attribute Lists 사용

Jekyll은 Attribute Lists를 지원하기 때문에 이를 이용할 수 있습니다. 예를 들어:

```markdown
![sample image](image.jpg){: width="300" height="200"}

```

위와 같이 Attribute Lists를 사용하여 이미지의 너비와 높이를 설정할 수 있습니다.

🔗 [Github 블로그에 이미지 넣기](https://seong6496.tistory.com/311)

### 예시 코드

다음은 Jekyll Now 블로그 포스트에 이미지를 삽입하고 크기를 조절하는 예시 코드입니다.

```markdown
---
layout: post
title: "이미지 크기 조절 예시"
date: 2024-07-05
---

## HTML 태그를 사용한 이미지 삽입
<img src="image.jpg" alt="sample image" width="300" height="200" />

## 스타일 속성을 사용한 이미지 삽입
<img src="image.jpg" alt="sample image" style="width:300px; height:200px;"/>

## Jekyll Attribute Lists를 사용한 이미지 삽입
![sample image](image.jpg){: width="300" height="200"}

```

위 예시 코드는 블로그 포스트 작성 시 다양한 방법으로 이미지를 삽입하고 크기를 조절하는 방법을 보여줍니다. Markdown의 유연성을 활용하여 HTML 태그나 Attribute Lists를 자유롭게 사용할 수 있습니다.

----------

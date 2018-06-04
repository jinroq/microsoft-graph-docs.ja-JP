# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="7e528-101">OneDrive ファイル ストレージ API の概要</span><span class="sxs-lookup"><span data-stu-id="7e528-101">OneDrive file storage API overview</span></span>

<span data-ttu-id="7e528-102">OneDrive は、Office 365 のファイル ハブです。</span><span class="sxs-lookup"><span data-stu-id="7e528-102">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="7e528-103">ファイルは、Microsoft Teams、グループ、SharePoint など、さまざまなコンテキストで利用されています。</span><span class="sxs-lookup"><span data-stu-id="7e528-103">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="7e528-104">OneDrive によりユーザーは、保存場所に関係なくそれらのファイルにアクセスすることができ、Microsoft Graph を使用すれば、単一の API でそれを操作できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-104">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="7e528-105">Office 365 のファイルは[ドライブ][Drive API]に保存されています。</span><span class="sxs-lookup"><span data-stu-id="7e528-105">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="7e528-106">ユーザーは、ファイルを個人的なドライブ - 自分の OneDrive - または [SharePoint][] ドキュメント ライブラリを利用した共有ドライブに保存できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-106">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="7e528-107">OneDrive の柔軟性のおかげで、ユーザーは、それぞれにとって最適な方法で共同作業をすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e528-107">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="7e528-108">ユーザーは、ファイルへのリンクを共有したり、ファイルをチーム ドライブにコピーまたは移動したり、Outlook で OneDrive ファイルをメール メッセージに添付したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e528-108">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="7e528-109">OneDrive ファイル ストレージをクラウドに統合する理由</span><span class="sxs-lookup"><span data-stu-id="7e528-109">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="7e528-110">何十億ものファイルをエコシステムで管理する</span><span class="sxs-lookup"><span data-stu-id="7e528-110">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="7e528-111">OneDrive ユーザーは、任意のデバイスから、オンラインまたはオフラインでファイルにアクセスすることができ、組織内外の人とファイルを共有することができます</span><span class="sxs-lookup"><span data-stu-id="7e528-111">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="7e528-112">OneDrive を利用すれば、Word、Excel、PowerPoint などの慣れ親しんだアプリを使用してリアルタイムで共同作成できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-112">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="7e528-113">Microsoft Graph によりファイルに対しては、何百種類もの形式の豊富なサムネイル、ビデオ ストリーミング、分析などの機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-113">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="7e528-114">OneDrive のデータは、ユーザーが信頼する方法で、高度な暗号化、コンプライアンス、およびセキュリティの機能によって保護されます。</span><span class="sxs-lookup"><span data-stu-id="7e528-114">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="7e528-115">OneDrive アプリは 5 億を超えるデバイスで実行されており、Fortune 500 企業の 85% 以上が OneDrive for Business を使用しています。アプリを OneDrive に統合することにより、すでにそこで日常的に作業を実行している何百万というユーザー、学生、およびビジネス ユーザーとつながって、彼らを関係付けることができます。</span><span class="sxs-lookup"><span data-stu-id="7e528-115">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="7e528-116">アプリのファイルを強力なクラウドに保存する</span><span class="sxs-lookup"><span data-stu-id="7e528-116">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="7e528-117">ファイルを OneDrive に保存すると、アプリで Microsoft クラウドのさまざまな機能を利用することができ、ユーザーはどこからでも自分のファイルにアクセスすることができるようになります。</span><span class="sxs-lookup"><span data-stu-id="7e528-117">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="7e528-118">[ファイル ピッカー][] SDK を使用することにより、OneDrive のユーザーが慣れ親しんでいるのと同じエクスペリエンスを使用して、独自のアプリ内から、OneDrive 内のファイルを開いたり、ダウンロードしたり、保存したり、共有したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e528-118">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="7e528-119">選択されたファイルに関する情報を、ファイル選択 SDK から直接取得したり、Microsoft Graph API を直接使用してファイルに関する深い対話操作を実行したりします。</span><span class="sxs-lookup"><span data-stu-id="7e528-119">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="7e528-120">[特殊フォルダー][]を使用して、`Documents` や `Camera Roll` など、OneDrive 上のよく知られた場所にファイルを保存したり、アプリに独自の個人用フォルダーを割り当てたりします。</span><span class="sxs-lookup"><span data-stu-id="7e528-120">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="7e528-121">OneDrive 内からユーザーに対してアプリを直接立ち上げる</span><span class="sxs-lookup"><span data-stu-id="7e528-121">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="7e528-122">OneDrive を使用する顧客は、OneDrive 内から直接アプリを使用または立ち上げて、ファイルを開いたり、編集したり、プレビューしたりできます。</span><span class="sxs-lookup"><span data-stu-id="7e528-122">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="7e528-123">OneDrive の[ファイル ハンドラー][]拡張機能を使用することにより、独自のカスタム ファイル拡張子に対してアイコンやプレビュー機能を提供したり、アプリを **[新規]** ボタンに追加したり、独自のカスタム アクションをメニュー バーに追加してアプリが起動するようにしたりできます。</span><span class="sxs-lookup"><span data-stu-id="7e528-123">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="7e528-124">アプリの認識する形式でコンテンツを処理する</span><span class="sxs-lookup"><span data-stu-id="7e528-124">Work with content in formats your app understands</span></span>

<span data-ttu-id="7e528-125">アプリは、最も都合の良い形式でファイルの内容を取得できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-125">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="7e528-126">アプリでは、何百という異なるファイル形式のために、カスタム サイズの[サムネイル][]を表示できます。</span><span class="sxs-lookup"><span data-stu-id="7e528-126">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="7e528-127">PDF など、さまざまな代替[形式][]でファイルをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="7e528-127">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="7e528-128">[プレビュー][] API (ベータ版) を使用することにより、OneDrive ファイルのプレビューをアプリ内に埋め込むこともできます。</span><span class="sxs-lookup"><span data-stu-id="7e528-128">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="7e528-129">バイナリをダウンロードすることなくファイルの内容およびメタデータを処理する</span><span class="sxs-lookup"><span data-stu-id="7e528-129">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="7e528-130">Microsoft Graph を利用すれば、バイナリをダウンロードしなくても、REST API を通じて、豊かな内容にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="7e528-130">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="7e528-131">[写真][]、[オーディオ][]、および [ビデオ][]のファイルから抽出したメタデータを調べます。</span><span class="sxs-lookup"><span data-stu-id="7e528-131">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="7e528-132">[Excel API][] は、Excel ブックに保存されている生のデータを直接操作するために使用します。</span><span class="sxs-lookup"><span data-stu-id="7e528-132">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="7e528-133">[Notes API][] は、OneNote のノートブックの内容にアクセスするために使用します。</span><span class="sxs-lookup"><span data-stu-id="7e528-133">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="7e528-134">ファイルへの変更に対応する</span><span class="sxs-lookup"><span data-stu-id="7e528-134">React to file changes</span></span>

<span data-ttu-id="7e528-135">アプリは [webhooks][] によって、ファイルに変更が加えられた時点で通知を受け取り、それに短時間で対応することができます。</span><span class="sxs-lookup"><span data-stu-id="7e528-135">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="7e528-136">[delta API][] を使用することにより、アプリがクラウドと同期した最後の時点以降で、どのような変更が加えられたかを調べます。</span><span class="sxs-lookup"><span data-stu-id="7e528-136">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7e528-137">次の手順</span><span class="sxs-lookup"><span data-stu-id="7e528-137">Next steps</span></span>

<span data-ttu-id="7e528-138">Microsoft Graph v1.0 における [OneDrive API の使用][Drive API]に関する詳細を確認する。</span><span class="sxs-lookup"><span data-stu-id="7e528-138">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[ファイル ピッカー]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[File picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[ファイル ハンドラー]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
<span data-ttu-id="7e528-142">
  [特殊フォルダー]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span><span class="sxs-lookup"><span data-stu-id="7e528-142">[Special folders]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span></span>
<span data-ttu-id="7e528-143">
  [メモ API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span><span class="sxs-lookup"><span data-stu-id="7e528-143">[Notes API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span></span>
<span data-ttu-id="7e528-144">
  [Excel API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span><span class="sxs-lookup"><span data-stu-id="7e528-144">[Excel API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span></span>
[REST API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
<span data-ttu-id="7e528-145">
  [delta API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span><span class="sxs-lookup"><span data-stu-id="7e528-145">[delta API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span></span>
<span data-ttu-id="7e528-146">
  [ビデオ]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span><span class="sxs-lookup"><span data-stu-id="7e528-146">[video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span></span>
<span data-ttu-id="7e528-147">
  [写真]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span><span class="sxs-lookup"><span data-stu-id="7e528-147">[photo]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span></span>
<span data-ttu-id="7e528-148">
  [オーディオ]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span><span class="sxs-lookup"><span data-stu-id="7e528-148">[audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span></span>
<span data-ttu-id="7e528-149">
  [形式]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span><span class="sxs-lookup"><span data-stu-id="7e528-149">[Formats]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span></span>
<span data-ttu-id="7e528-150">
  [サムネイル]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span><span class="sxs-lookup"><span data-stu-id="7e528-150">[thumbnails]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span></span>
<span data-ttu-id="7e528-151">
  [プレビュー]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span><span class="sxs-lookup"><span data-stu-id="7e528-151">[Preview]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span></span>
<span data-ttu-id="7e528-152">
  [webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span><span class="sxs-lookup"><span data-stu-id="7e528-152">[Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span></span>
[Drive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive

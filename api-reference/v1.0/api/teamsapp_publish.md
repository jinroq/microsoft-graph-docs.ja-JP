# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="1d134-101">アプリケーションを組織のアプリケーションのカタログに発行します。</span><span class="sxs-lookup"><span data-stu-id="1d134-101">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="1d134-102">マイクロソフト チーム アプリケーション カタログに[アプリケーション](../resources/teamsapp.md)を発行します。</span><span class="sxs-lookup"><span data-stu-id="1d134-102">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="1d134-103">この API が、アプリケーションを公開して、組織のカタログ (テナント アプリケーション カタログ) に具体的には、作成されたリソースがある`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="1d134-103">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d134-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d134-104">Permissions</span></span>

<span data-ttu-id="1d134-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d134-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="1d134-107">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="1d134-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="1d134-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d134-108">Permission Type</span></span>                        | <span data-ttu-id="1d134-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d134-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="1d134-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d134-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d134-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d134-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="1d134-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d134-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d134-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1d134-113">Not supported</span></span>|
| <span data-ttu-id="1d134-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d134-114">Application</span></span>                            | <span data-ttu-id="1d134-115">非サポート</span><span class="sxs-lookup"><span data-stu-id="1d134-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d134-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d134-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="1d134-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d134-117">Request headers</span></span>

| <span data-ttu-id="1d134-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d134-118">Header</span></span>        | <span data-ttu-id="1d134-119">値</span><span class="sxs-lookup"><span data-stu-id="1d134-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="1d134-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d134-120">Authorization</span></span> | <span data-ttu-id="1d134-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d134-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d134-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d134-123">Content-Type</span></span>  | <span data-ttu-id="1d134-124">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="1d134-124">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d134-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d134-125">Request body</span></span>

<span data-ttu-id="1d134-126">チーム Zip のマニフェスト ペイロード。</span><span class="sxs-lookup"><span data-stu-id="1d134-126">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="1d134-127">チームのアプリケーションのファイルは[、アプリケーション パッケージの作成を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)zip 形式で圧縮します。</span><span class="sxs-lookup"><span data-stu-id="1d134-127">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="1d134-128">その組織の別のアプリケーションと同じマニフェスト ID を持つ組織のアプリケーションを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="1d134-128">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="1d134-129">応答</span><span class="sxs-lookup"><span data-stu-id="1d134-129">Response</span></span>

<span data-ttu-id="1d134-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと[teamsCatalogApp](../resources/teamsapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1d134-130">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="1d134-131">例</span><span class="sxs-lookup"><span data-stu-id="1d134-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d134-132">要求</span><span class="sxs-lookup"><span data-stu-id="1d134-132">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="1d134-133">マイクロソフト チームのアプリケーションの zip ファイルを作成する方法の詳細については、[作成されたアプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d134-133">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="1d134-134">応答</span><span class="sxs-lookup"><span data-stu-id="1d134-134">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

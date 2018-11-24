# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="e7cd8-101">組織のアプリケーションのカタログからアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-101">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="e7cd8-102">組織のアプリケーション カタログ (テナント アプリケーション カタログ) から[アプリケーション](../resources/teamsapp.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-102">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e7cd8-103">組織のアプリケーションのカタログからアプリケーションを削除するのには次のように指定します。 `organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-103">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7cd8-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7cd8-104">Permissions</span></span>

<span data-ttu-id="e7cd8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e7cd8-107">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="e7cd8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7cd8-108">Permission Type</span></span>                        | <span data-ttu-id="e7cd8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7cd8-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e7cd8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7cd8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7cd8-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7cd8-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e7cd8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7cd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7cd8-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e7cd8-113">Not supported</span></span>|
| <span data-ttu-id="e7cd8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7cd8-114">Application</span></span>                            | <span data-ttu-id="e7cd8-115">非サポート</span><span class="sxs-lookup"><span data-stu-id="e7cd8-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7cd8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7cd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7cd8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7cd8-117">Request headers</span></span>

| <span data-ttu-id="e7cd8-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7cd8-118">Header</span></span>        | <span data-ttu-id="e7cd8-119">値</span><span class="sxs-lookup"><span data-stu-id="e7cd8-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e7cd8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7cd8-120">Authorization</span></span> | <span data-ttu-id="e7cd8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7cd8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7cd8-123">Request body</span></span>

<span data-ttu-id="e7cd8-124">なし。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-124">None.</span></span>

><span data-ttu-id="e7cd8-125">**注:** 更新するにはアプリケーションを参照するための[リストには、アプリケーションが公開されて](./teamsapp_list.md)呼び出しから返された ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-125">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e7cd8-126">Zip アプリケーション パッケージのマニフェストの ID を使用しません。</span><span class="sxs-lookup"><span data-stu-id="e7cd8-126">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e7cd8-127">応答</span><span class="sxs-lookup"><span data-stu-id="e7cd8-127">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e7cd8-128">例</span><span class="sxs-lookup"><span data-stu-id="e7cd8-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7cd8-129">要求</span><span class="sxs-lookup"><span data-stu-id="e7cd8-129">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="e7cd8-130">応答</span><span class="sxs-lookup"><span data-stu-id="e7cd8-130">Response</span></span>

```http
HTTP/1.1 204 No Content
```

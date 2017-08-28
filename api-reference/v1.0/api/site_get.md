# <a name="get-a-site-resource"></a><span data-ttu-id="1015e-101">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="1015e-101">Get a site resource</span></span>

<span data-ttu-id="1015e-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="1015e-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="1015e-104">[サイト]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="1015e-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="1015e-105">**サイト**は、以下の値の複合 ID である、一意識別子にアドレス指定されます。</span><span class="sxs-lookup"><span data-stu-id="1015e-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="1015e-106">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="1015e-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="1015e-107">サイト コレクションの一意 ID (guid)</span><span class="sxs-lookup"><span data-stu-id="1015e-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="1015e-108">サイトの一意 ID (guid)</span><span class="sxs-lookup"><span data-stu-id="1015e-108">Site unique ID (guid)</span></span>

<span data-ttu-id="1015e-109">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="1015e-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="1015e-110">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="1015e-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="1015e-111">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="1015e-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="1015e-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1015e-112">Permissions</span></span>

<span data-ttu-id="1015e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1015e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1015e-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1015e-115">Permission type</span></span>      | <span data-ttu-id="1015e-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1015e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1015e-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1015e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1015e-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1015e-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1015e-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1015e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1015e-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1015e-120">Not supported.</span></span>    |
|<span data-ttu-id="1015e-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1015e-121">Application</span></span> | <span data-ttu-id="1015e-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1015e-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="1015e-123">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="1015e-123">Get the tenant's root site</span></span>

<span data-ttu-id="1015e-124">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1015e-124">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="1015e-125">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="1015e-125">Access a site by server-relative URL</span></span>

<span data-ttu-id="1015e-126">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="1015e-126">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="1015e-127">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="1015e-127">Access a group team site</span></span>

<span data-ttu-id="1015e-128">[グループ](../resources/group.md) のチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1015e-128">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="1015e-129">例</span><span class="sxs-lookup"><span data-stu-id="1015e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1015e-130">要求</span><span class="sxs-lookup"><span data-stu-id="1015e-130">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="1015e-131">応答</span><span class="sxs-lookup"><span data-stu-id="1015e-131">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->

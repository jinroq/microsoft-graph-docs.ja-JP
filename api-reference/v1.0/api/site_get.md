# <a name="get-a-site-resource"></a><span data-ttu-id="a071d-101">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="a071d-101">Get a site resource</span></span>

<span data-ttu-id="a071d-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="a071d-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="a071d-104">[サイト]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="a071d-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="a071d-105">**サイト**は、以下の値の複合 ID である、一意識別子にアドレス指定されます。</span><span class="sxs-lookup"><span data-stu-id="a071d-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="a071d-106">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="a071d-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="a071d-107">サイト コレクションの一意 ID (guid)</span><span class="sxs-lookup"><span data-stu-id="a071d-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="a071d-108">サイトの一意 ID (guid)</span><span class="sxs-lookup"><span data-stu-id="a071d-108">Site unique ID (guid)</span></span>

<span data-ttu-id="a071d-109">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="a071d-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="a071d-110">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="a071d-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="a071d-111">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="a071d-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a071d-112">前提条件</span><span class="sxs-lookup"><span data-stu-id="a071d-112">Prerequisites</span></span>

<span data-ttu-id="a071d-113">この要求を実行するには、以下のいずれかのスコープが必要です。</span><span class="sxs-lookup"><span data-stu-id="a071d-113">One of the following scopes is required to execute this request:</span></span>

* <span data-ttu-id="a071d-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a071d-114">Sites.Read.All</span></span>
* <span data-ttu-id="a071d-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a071d-115">Sites.ReadWrite.All</span></span>

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="a071d-116">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="a071d-116">Get the tenant's root site</span></span>

<span data-ttu-id="a071d-117">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a071d-117">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="a071d-118">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a071d-118">Access a site by server-relative URL</span></span>

<span data-ttu-id="a071d-119">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="a071d-119">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="a071d-120">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a071d-120">Access a group team site</span></span>

<span data-ttu-id="a071d-121">[グループ](../resources/group.md) のチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a071d-121">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="a071d-122">例</span><span class="sxs-lookup"><span data-stu-id="a071d-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a071d-123">要求</span><span class="sxs-lookup"><span data-stu-id="a071d-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="a071d-124">応答</span><span class="sxs-lookup"><span data-stu-id="a071d-124">Response</span></span>

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

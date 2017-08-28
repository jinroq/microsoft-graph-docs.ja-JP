# <a name="enumerate-subsites-of-a-site"></a><span data-ttu-id="8dc21-101">サイトのサブサイトを列挙する</span><span class="sxs-lookup"><span data-stu-id="8dc21-101">Enumerate subsites of a site</span></span>

<span data-ttu-id="8dc21-102">[site][] に定義されているサブサイトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8dc21-102">Get a collection of subsites defined for a [site][].</span></span>

<span data-ttu-id="8dc21-103">[サイト]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="8dc21-103">[site]: ../resources/site.md</span></span>

## <a name="permissions"></a><span data-ttu-id="8dc21-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8dc21-104">Permissions</span></span>

<span data-ttu-id="8dc21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8dc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8dc21-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8dc21-107">Permission type</span></span>      | <span data-ttu-id="8dc21-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8dc21-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dc21-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8dc21-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8dc21-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc21-110">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8dc21-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8dc21-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dc21-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dc21-112">Not supported.</span></span>    |
|<span data-ttu-id="8dc21-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8dc21-113">Application</span></span> | <span data-ttu-id="8dc21-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc21-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dc21-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8dc21-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

## <a name="example"></a><span data-ttu-id="8dc21-116">例</span><span class="sxs-lookup"><span data-stu-id="8dc21-116">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8dc21-117">要求</span><span class="sxs-lookup"><span data-stu-id="8dc21-117">Request</span></span>

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a><span data-ttu-id="8dc21-118">応答</span><span class="sxs-lookup"><span data-stu-id="8dc21-118">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Enumerate subsites"
} -->

# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="60459-101">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60459-101">teamsAppDefinition resource type</span></span>



<span data-ttu-id="60459-102">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="60459-102">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="60459-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60459-103">Properties</span></span>

| <span data-ttu-id="60459-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60459-104">Property</span></span>            | <span data-ttu-id="60459-105">型</span><span class="sxs-lookup"><span data-stu-id="60459-105">Type</span></span>     | <span data-ttu-id="60459-106">説明</span><span class="sxs-lookup"><span data-stu-id="60459-106">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="60459-107">ID</span><span class="sxs-lookup"><span data-stu-id="60459-107">id</span></span>                  | <span data-ttu-id="60459-108">文字列</span><span class="sxs-lookup"><span data-stu-id="60459-108">string</span></span>   | <span data-ttu-id="60459-109">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="60459-109">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="60459-110">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="60459-110">teamsAppId</span></span>          | <span data-ttu-id="60459-111">文字列</span><span class="sxs-lookup"><span data-stu-id="60459-111">string</span></span>   | <span data-ttu-id="60459-112">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="60459-112">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="60459-113">displayName</span><span class="sxs-lookup"><span data-stu-id="60459-113">displayName</span></span>         | <span data-ttu-id="60459-114">string</span><span class="sxs-lookup"><span data-stu-id="60459-114">string</span></span>   | <span data-ttu-id="60459-115">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="60459-115">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="60459-116">version</span><span class="sxs-lookup"><span data-stu-id="60459-116">version</span></span>             | <span data-ttu-id="60459-117">文字列</span><span class="sxs-lookup"><span data-stu-id="60459-117">string</span></span>   | <span data-ttu-id="60459-118">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="60459-118">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60459-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60459-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="60459-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="60459-120">See also</span></span>

- [<span data-ttu-id="60459-121">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60459-121">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="60459-122">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="60459-122">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="60459-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60459-123">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


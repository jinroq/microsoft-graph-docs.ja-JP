# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="c3773-101">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3773-101">teamsAppInstallation resource type</span></span>



<span data-ttu-id="c3773-102">[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c3773-102">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="c3773-103">アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。</span><span class="sxs-lookup"><span data-stu-id="c3773-103">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="c3773-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3773-104">Methods</span></span>

| <span data-ttu-id="c3773-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3773-105">Method</span></span>       | <span data-ttu-id="c3773-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c3773-106">Return Type</span></span>  |<span data-ttu-id="c3773-107">説明</span><span class="sxs-lookup"><span data-stu-id="c3773-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3773-108">リスト アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3773-108">List apps</span></span>](../api/teamsappinstallation_list.md) | [<span data-ttu-id="c3773-109">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c3773-109">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c3773-110">チームでインストールされているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c3773-110">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="c3773-111">アプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="c3773-111">Add app</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="c3773-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c3773-112">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c3773-113">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="c3773-113">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="c3773-114">アプリを抹消します。</span><span class="sxs-lookup"><span data-stu-id="c3773-114">Remove app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="c3773-115">なし</span><span class="sxs-lookup"><span data-stu-id="c3773-115">None</span></span> | <span data-ttu-id="c3773-116">削除 (アンインストール)、チームからのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="c3773-116">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="c3773-117">アプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="c3773-117">Upgrade app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="c3773-118">なし</span><span class="sxs-lookup"><span data-stu-id="c3773-118">None</span></span> | <span data-ttu-id="c3773-119">アプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="c3773-119">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3773-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3773-120">Properties</span></span>

| <span data-ttu-id="c3773-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3773-121">Property</span></span>            | <span data-ttu-id="c3773-122">型</span><span class="sxs-lookup"><span data-stu-id="c3773-122">Type</span></span>     | <span data-ttu-id="c3773-123">説明</span><span class="sxs-lookup"><span data-stu-id="c3773-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c3773-124">ID</span><span class="sxs-lookup"><span data-stu-id="c3773-124">id</span></span>                  | <span data-ttu-id="c3773-125">文字列</span><span class="sxs-lookup"><span data-stu-id="c3773-125">string</span></span>   | <span data-ttu-id="c3773-126">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="c3773-126">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3773-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3773-127">Relationships</span></span>

| <span data-ttu-id="c3773-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3773-128">Relationship</span></span>   | <span data-ttu-id="c3773-129">型</span><span class="sxs-lookup"><span data-stu-id="c3773-129">Type</span></span>    | <span data-ttu-id="c3773-130">説明</span><span class="sxs-lookup"><span data-stu-id="c3773-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c3773-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c3773-131">teamsApp</span></span>|[<span data-ttu-id="c3773-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c3773-132">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="c3773-133">インストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="c3773-133">The app that is installed.</span></span> |
|<span data-ttu-id="c3773-134">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c3773-134">teamsAppDefinition</span></span>|[<span data-ttu-id="c3773-135">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c3773-135">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="c3773-136">このバージョンのアプリケーションの詳細。</span><span class="sxs-lookup"><span data-stu-id="c3773-136">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3773-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3773-137">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="c3773-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3773-138">See also</span></span>

- [<span data-ttu-id="c3773-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c3773-139">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="c3773-140">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c3773-140">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c3773-141">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c3773-141">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


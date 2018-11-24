# <a name="teamsapp-resource-type"></a><span data-ttu-id="e64f0-101">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e64f0-101">teamsApp resource type</span></span>



<span data-ttu-id="e64f0-102">[マイクロソフト チーム](teams_api_overview.md)アプリケーション カタログのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="e64f0-102">An app in the [Microsoft Teams](teams_api_overview.md) app catalog.</span></span>

<span data-ttu-id="e64f0-103">マイクロソフト チーム ストア内のこれらのアプリケーションを表示して、[チーム](team.md)が[チームに追加のアプリケーション](../api/teamsappinstallation_add.md)のメソッドを使用してこれらのアプリケーションをインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="e64f0-103">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation_add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="e64f0-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e64f0-104">Methods</span></span>

| <span data-ttu-id="e64f0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e64f0-105">Method</span></span>       | <span data-ttu-id="e64f0-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e64f0-106">Return Type</span></span>  |<span data-ttu-id="e64f0-107">説明</span><span class="sxs-lookup"><span data-stu-id="e64f0-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e64f0-108">公開されたアプリケーションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-108">List published apps</span></span>](../api/teamsapp_list.md) | <span data-ttu-id="e64f0-109">[teamsApp](teamsApp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e64f0-109">[teamsApp](teamsApp.md) collection</span></span> | <span data-ttu-id="e64f0-110">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-110">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="e64f0-111">アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-111">Publish an app</span></span>](../api/teamsapp_publish.md) | [<span data-ttu-id="e64f0-112">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e64f0-112">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="e64f0-113">組織のアプリケーションのカタログには、アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-113">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="e64f0-114">発行したアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-114">Update a published app</span></span>](../api/teamsapp_update.md) | [<span data-ttu-id="e64f0-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e64f0-115">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="e64f0-116">組織のアプリケーションのカタログに公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-116">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="e64f0-117">発行したアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-117">Remove a published app</span></span>](../api/teamsapp_delete.md) | <span data-ttu-id="e64f0-118">なし</span><span class="sxs-lookup"><span data-stu-id="e64f0-118">None</span></span> | <span data-ttu-id="e64f0-119">発行したアプリケーションを組織のアプリケーションのカタログから削除します。</span><span class="sxs-lookup"><span data-stu-id="e64f0-119">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="e64f0-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64f0-120">Properties</span></span>

| <span data-ttu-id="e64f0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64f0-121">Property</span></span>            | <span data-ttu-id="e64f0-122">型</span><span class="sxs-lookup"><span data-stu-id="e64f0-122">Type</span></span>     | <span data-ttu-id="e64f0-123">説明</span><span class="sxs-lookup"><span data-stu-id="e64f0-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e64f0-124">ID</span><span class="sxs-lookup"><span data-stu-id="e64f0-124">id</span></span>                  | <span data-ttu-id="e64f0-125">文字列</span><span class="sxs-lookup"><span data-stu-id="e64f0-125">string</span></span>   | <span data-ttu-id="e64f0-126">カタログ アプリケーションの生成のアプリケーション ID を ([マイクロソフト チーム zip アプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者から提供された ID とは異なる。</span><span class="sxs-lookup"><span data-stu-id="e64f0-126">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e64f0-127">externalId</span><span class="sxs-lookup"><span data-stu-id="e64f0-127">externalId</span></span>          | <span data-ttu-id="e64f0-128">文字列</span><span class="sxs-lookup"><span data-stu-id="e64f0-128">string</span></span>   | <span data-ttu-id="e64f0-129">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログの ID です。</span><span class="sxs-lookup"><span data-stu-id="e64f0-129">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e64f0-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e64f0-130">displayName</span></span>                | <span data-ttu-id="e64f0-131">string</span><span class="sxs-lookup"><span data-stu-id="e64f0-131">string</span></span>   | <span data-ttu-id="e64f0-132">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログのアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e64f0-132">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e64f0-133">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="e64f0-133">distributionMethod</span></span>  | <span data-ttu-id="e64f0-134">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="e64f0-134">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="e64f0-135">アプリケーション配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="e64f0-135">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="e64f0-136">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="e64f0-136">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="e64f0-137">メンバー</span><span class="sxs-lookup"><span data-stu-id="e64f0-137">Member</span></span>|<span data-ttu-id="e64f0-138">値</span><span class="sxs-lookup"><span data-stu-id="e64f0-138">Value</span></span>|<span data-ttu-id="e64f0-139">説明</span><span class="sxs-lookup"><span data-stu-id="e64f0-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e64f0-140">ストア</span><span class="sxs-lookup"><span data-stu-id="e64f0-140">store</span></span>|<span data-ttu-id="e64f0-141">0</span><span class="sxs-lookup"><span data-stu-id="e64f0-141">0</span></span>| <span data-ttu-id="e64f0-142">アプリケーションは、マイクロソフトのチームのアプリケーション ストアからのすべてのテナントに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e64f0-142">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="e64f0-143">組織</span><span class="sxs-lookup"><span data-stu-id="e64f0-143">organization</span></span>|<span data-ttu-id="e64f0-144">1</span><span class="sxs-lookup"><span data-stu-id="e64f0-144">1</span></span>|<span data-ttu-id="e64f0-145">アプリケーションは、このテナントでのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="e64f0-145">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="e64f0-146">sideloaded</span><span class="sxs-lookup"><span data-stu-id="e64f0-146">sideloaded</span></span>|<span data-ttu-id="e64f0-147">2</span><span class="sxs-lookup"><span data-stu-id="e64f0-147">2</span></span>|<span data-ttu-id="e64f0-148">アプリケーションは、ユーザーまたはチームのみ使用可能です、インストールされているをします。</span><span class="sxs-lookup"><span data-stu-id="e64f0-148">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e64f0-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e64f0-149">Relationships</span></span>

| <span data-ttu-id="e64f0-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e64f0-150">Relationship</span></span> | <span data-ttu-id="e64f0-151">型</span><span class="sxs-lookup"><span data-stu-id="e64f0-151">Type</span></span>   | <span data-ttu-id="e64f0-152">説明</span><span class="sxs-lookup"><span data-stu-id="e64f0-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e64f0-153">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="e64f0-153">appDefinitions</span></span>|<span data-ttu-id="e64f0-154">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e64f0-154">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="e64f0-155">アプリケーションの各バージョンの詳細です。</span><span class="sxs-lookup"><span data-stu-id="e64f0-155">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e64f0-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e64f0-156">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a><span data-ttu-id="e64f0-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="e64f0-157">See also</span></span>

- [<span data-ttu-id="e64f0-158">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e64f0-158">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e64f0-159">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e64f0-159">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e64f0-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e64f0-160">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="1bbee-101">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bbee-101">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="1bbee-102"> [user](user.md) エンティティの **onPremisesExtensionAttributes** プロパティは、15 個のカスタム拡張機能の属性のプロパティを含みます。</span><span class="sxs-lookup"><span data-stu-id="1bbee-102">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="1bbee-103">**onPremisesSyncEnabled** のユーザーでは、このプロパティのセットは内部設置型の Active Directory をマスタとし、Azure AD に同期され、読み取り専用となります。</span><span class="sxs-lookup"><span data-stu-id="1bbee-103">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="1bbee-104">クラウドのみのユーザー (**onPremisesSyncEnabled** が falseの場合) では、これらのプロパティは作成時または更新時に設定されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1bbee-104">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="1bbee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bbee-105">Properties</span></span>
| <span data-ttu-id="1bbee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bbee-106">Property</span></span>     | <span data-ttu-id="1bbee-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="1bbee-107">Type</span></span>   |<span data-ttu-id="1bbee-108">説明</span><span class="sxs-lookup"><span data-stu-id="1bbee-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bbee-109">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="1bbee-109">extensionAttribute1</span></span>|<span data-ttu-id="1bbee-110">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-110">String</span></span>| <span data-ttu-id="1bbee-111">最初のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-111">First customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-112">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="1bbee-112">extensionAttribute2</span></span>|<span data-ttu-id="1bbee-113">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-113">String</span></span>| <span data-ttu-id="1bbee-114">2 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-114">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-115">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="1bbee-115">extensionAttribute3</span></span>|<span data-ttu-id="1bbee-116">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-116">String</span></span>| <span data-ttu-id="1bbee-117">3 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-117">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-118">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="1bbee-118">extensionAttribute4</span></span>|<span data-ttu-id="1bbee-119">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-119">String</span></span>| <span data-ttu-id="1bbee-120">4 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-120">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-121">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="1bbee-121">extensionAttribute5</span></span>|<span data-ttu-id="1bbee-122">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-122">String</span></span>| <span data-ttu-id="1bbee-123">5 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-123">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-124">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="1bbee-124">extensionAttribute6</span></span>|<span data-ttu-id="1bbee-125">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-125">String</span></span>| <span data-ttu-id="1bbee-126">6 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-126">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-127">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="1bbee-127">extensionAttribute7</span></span>|<span data-ttu-id="1bbee-128">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-128">String</span></span>| <span data-ttu-id="1bbee-129">7 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-129">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-130">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="1bbee-130">extensionAttribute8</span></span>|<span data-ttu-id="1bbee-131">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-131">String</span></span>| <span data-ttu-id="1bbee-132">8 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-132">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-133">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="1bbee-133">extensionAttribute9</span></span>|<span data-ttu-id="1bbee-134">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-134">String</span></span>| <span data-ttu-id="1bbee-135">9 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-135">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-136">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="1bbee-136">extensionAttribute10</span></span>|<span data-ttu-id="1bbee-137">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-137">String</span></span>| <span data-ttu-id="1bbee-138">10 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-138">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-139">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="1bbee-139">extensionAttribute11</span></span>|<span data-ttu-id="1bbee-140">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-140">String</span></span>| <span data-ttu-id="1bbee-141">11 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-141">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-142">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="1bbee-142">extensionAttribute12</span></span>|<span data-ttu-id="1bbee-143">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-143">String</span></span>| <span data-ttu-id="1bbee-144">12 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-144">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-145">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="1bbee-145">extensionAttribute13</span></span>|<span data-ttu-id="1bbee-146">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-146">String</span></span>| <span data-ttu-id="1bbee-147">13 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-147">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-148">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="1bbee-148">extensionAttribute14</span></span>|<span data-ttu-id="1bbee-149">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-149">String</span></span>| <span data-ttu-id="1bbee-150">14 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-150">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1bbee-151">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="1bbee-151">extensionAttribute15</span></span>|<span data-ttu-id="1bbee-152">String</span><span class="sxs-lookup"><span data-stu-id="1bbee-152">String</span></span>| <span data-ttu-id="1bbee-153">15 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1bbee-153">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bbee-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1bbee-154">JSON representation</span></span>

<span data-ttu-id="1bbee-155">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1bbee-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
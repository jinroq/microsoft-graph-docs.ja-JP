---
title: リソースの種類を配置する
description: 場所を表します。 これは、room または roomList の基本型です。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5cea04931d537c8b0bd29c49327a56afe8a7d5d5
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841298"
---
# <a name="place-resource-type"></a><span data-ttu-id="febcd-104">リソースの種類を配置する</span><span class="sxs-lookup"><span data-stu-id="febcd-104">place resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="febcd-105">名前、物理アドレス、地理的な座標などの基本的な場所の属性を表します。</span><span class="sxs-lookup"><span data-stu-id="febcd-105">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="febcd-106">これは、 [room](room.md)や[roomList](roomlist.md)などの豊富な場所の種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="febcd-106">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="febcd-107">プレース API の使用</span><span class="sxs-lookup"><span data-stu-id="febcd-107">Using the places API</span></span>
<span data-ttu-id="febcd-108">Exchange Online 管理者は、テナント内の会議室を会議室一覧にまとめることができます。</span><span class="sxs-lookup"><span data-stu-id="febcd-108">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="febcd-109">プレース API を使用すると、テナント内のすべての会議室一覧またはルームを取得したり、特定の会議室一覧のすべての会議室を取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="febcd-109">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="febcd-110">[Room](room.md)や[roomList](roomlist.md)などの場所には、基本**id**、表示名、電子メールアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="febcd-110">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="febcd-111">また、物理アドレスと地理的な座標、ルームの場合は、AV 能力、フロア番号、容量などの他の関連情報などのナビゲーション情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="febcd-111">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="febcd-112">[Findrooms](../api/user-findrooms.md)および[fin/omlists](../api/user-findroomlists.md)関数は、テナント内のルームおよび会議室一覧に類似した参照をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="febcd-112">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="febcd-113">以下に、プレース API とこれらの関数の比較を示します。</span><span class="sxs-lookup"><span data-stu-id="febcd-113">The following is a comparison between the places API and these functions.</span></span>

|<span data-ttu-id="febcd-114">配置 API</span><span class="sxs-lookup"><span data-stu-id="febcd-114">Places API</span></span> |<span data-ttu-id="febcd-115">Findrooms および fin/Omlists 関数</span><span class="sxs-lookup"><span data-stu-id="febcd-115">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="febcd-116">テナント内のすべての部屋または会議室一覧の取得、および会議室一覧のすべての会議室の取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="febcd-116">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="febcd-117">同様のサポート-テナント内のすべてのルームまたはルームリストと、ルームリスト内のすべてのルームを取得します。</span><span class="sxs-lookup"><span data-stu-id="febcd-117">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="febcd-118">[リストの場所](../api/place-list.md)がテナント内の100ルームを超えることがある</span><span class="sxs-lookup"><span data-stu-id="febcd-118">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="febcd-119">[Fin[oms](../api/user-findrooms.md)は、テナント内の最初の100ルームに戻る</span><span class="sxs-lookup"><span data-stu-id="febcd-119">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="febcd-120">テナント内の[個別の会議室または会議室一覧の取得](../api/place-get.md)をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="febcd-120">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="febcd-121">テナント内の個別の会議室または会議室一覧の取得はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="febcd-121">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="febcd-122">表示名と SMTP アドレスに加えて、豊富なプロパティセットを指定する[room](room.md)および[roomList](roomlist.md)の特定のエンティティを定義します。</span><span class="sxs-lookup"><span data-stu-id="febcd-122">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="febcd-123">各会議室および会議室一覧には、表示名と SMTP アドレスのみを指定する、軽量化された[emailAddress](emailaddress.md)の種類があります。</span><span class="sxs-lookup"><span data-stu-id="febcd-123">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="febcd-124">委任 (職場または学校のアカウント) またはアプリケーションのアクセス許可を持つ、組織のシナリオのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="febcd-124">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="febcd-125">委任されたアクセス許可またはアプリケーションのアクセス許可を持つ組織のシナリオに対して同様のサポート</span><span class="sxs-lookup"><span data-stu-id="febcd-125">Similar support for only organizational scenarios with delegated or application permissions</span></span>|

## <a name="methods"></a><span data-ttu-id="febcd-126">メソッド</span><span class="sxs-lookup"><span data-stu-id="febcd-126">Methods</span></span>

| <span data-ttu-id="febcd-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="febcd-127">Method</span></span>                              | <span data-ttu-id="febcd-128">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="febcd-128">Return Type</span></span>                  | <span data-ttu-id="febcd-129">説明</span><span class="sxs-lookup"><span data-stu-id="febcd-129">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="febcd-130">プレースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="febcd-130">List places</span></span>](../api/place-list.md) | <span data-ttu-id="febcd-131">要求された派生型のコレクション。 [](place.md)</span><span class="sxs-lookup"><span data-stu-id="febcd-131">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="febcd-132">テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="febcd-132">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="febcd-133">場所を取得する</span><span class="sxs-lookup"><span data-stu-id="febcd-133">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="febcd-134">要求された派生型[](place.md)</span><span class="sxs-lookup"><span data-stu-id="febcd-134">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="febcd-135">指定した**place**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="febcd-135">Get the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="febcd-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="febcd-136">Properties</span></span>

| <span data-ttu-id="febcd-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="febcd-137">Property</span></span>       | <span data-ttu-id="febcd-138">型</span><span class="sxs-lookup"><span data-stu-id="febcd-138">Type</span></span>                                              | <span data-ttu-id="febcd-139">説明</span><span class="sxs-lookup"><span data-stu-id="febcd-139">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="febcd-140">address</span><span class="sxs-lookup"><span data-stu-id="febcd-140">address</span></span>        | [<span data-ttu-id="febcd-141">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="febcd-141">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="febcd-142">場所の住所。</span><span class="sxs-lookup"><span data-stu-id="febcd-142">The street address of the place.</span></span> |
| <span data-ttu-id="febcd-143">displayName</span><span class="sxs-lookup"><span data-stu-id="febcd-143">displayName</span></span>    | <span data-ttu-id="febcd-144">String</span><span class="sxs-lookup"><span data-stu-id="febcd-144">String</span></span>                                            | <span data-ttu-id="febcd-145">場所に関連付けられている名前。</span><span class="sxs-lookup"><span data-stu-id="febcd-145">The name associated with the place.</span></span> |
| <span data-ttu-id="febcd-146">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="febcd-146">geoCoordinates</span></span> | [<span data-ttu-id="febcd-147">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="febcd-147">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="febcd-148">緯度、経度、および (オプションで) 高度座標での場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="febcd-148">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="febcd-149">id</span><span class="sxs-lookup"><span data-stu-id="febcd-149">id</span></span>             | <span data-ttu-id="febcd-150">文字列</span><span class="sxs-lookup"><span data-stu-id="febcd-150">String</span></span>                                            | <span data-ttu-id="febcd-151">場所の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="febcd-151">Unique identifier for the place.</span></span> <span data-ttu-id="febcd-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="febcd-152">Read-only.</span></span> |
| <span data-ttu-id="febcd-153">phone</span><span class="sxs-lookup"><span data-stu-id="febcd-153">phone</span></span>          | <span data-ttu-id="febcd-154">String</span><span class="sxs-lookup"><span data-stu-id="febcd-154">String</span></span>                                            | <span data-ttu-id="febcd-155">場所の電話番号。</span><span class="sxs-lookup"><span data-stu-id="febcd-155">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="febcd-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="febcd-156">Relationships</span></span>

<span data-ttu-id="febcd-157">なし。</span><span class="sxs-lookup"><span data-stu-id="febcd-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="febcd-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="febcd-158">JSON representation</span></span>

<span data-ttu-id="febcd-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="febcd-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a><span data-ttu-id="febcd-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="febcd-160">See also</span></span>
- <span data-ttu-id="febcd-161">管理者が会議室一覧を作成するには、Exchange PowerShell コマンドレットの[新しいグループ](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)を使用します。</span><span class="sxs-lookup"><span data-stu-id="febcd-161">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="febcd-162">管理者が会議室一覧に会議室を追加するには、Exchange Powershell コマンドレット[get-distributiongroupmember](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)を使用します。</span><span class="sxs-lookup"><span data-stu-id="febcd-162">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

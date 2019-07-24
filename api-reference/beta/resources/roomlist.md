---
title: roomList リソースの種類
description: 会社によって作成されたルームのグループを表します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841256"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="86ad7-103">roomList リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86ad7-103">roomList resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86ad7-104">テナントで定義されている[ルーム](room.md)オブジェクトのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="86ad7-104">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="86ad7-105">派生元[](place.md)。</span><span class="sxs-lookup"><span data-stu-id="86ad7-105">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="86ad7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="86ad7-106">Methods</span></span>

| <span data-ttu-id="86ad7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="86ad7-107">Method</span></span>                              | <span data-ttu-id="86ad7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86ad7-108">Return Type</span></span>                  | <span data-ttu-id="86ad7-109">説明</span><span class="sxs-lookup"><span data-stu-id="86ad7-109">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="86ad7-110">プレースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="86ad7-110">List places</span></span>](../api/place-list.md) | <span data-ttu-id="86ad7-111">要求された派生型のコレクション。 [](place.md)</span><span class="sxs-lookup"><span data-stu-id="86ad7-111">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="86ad7-112">テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="86ad7-112">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="86ad7-113">たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。</span><span class="sxs-lookup"><span data-stu-id="86ad7-113">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="86ad7-114">場所を取得する</span><span class="sxs-lookup"><span data-stu-id="86ad7-114">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="86ad7-115">要求された派生型[](place.md)</span><span class="sxs-lookup"><span data-stu-id="86ad7-115">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="86ad7-116">ルームリストなど、指定した**place**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="86ad7-116">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="86ad7-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86ad7-117">Properties</span></span>

| <span data-ttu-id="86ad7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86ad7-118">Property</span></span>       | <span data-ttu-id="86ad7-119">型</span><span class="sxs-lookup"><span data-stu-id="86ad7-119">Type</span></span>                                              | <span data-ttu-id="86ad7-120">説明</span><span class="sxs-lookup"><span data-stu-id="86ad7-120">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="86ad7-121">address</span><span class="sxs-lookup"><span data-stu-id="86ad7-121">address</span></span>        | [<span data-ttu-id="86ad7-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="86ad7-122">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="86ad7-123">会議室リストの住所。</span><span class="sxs-lookup"><span data-stu-id="86ad7-123">The street address of the room list.</span></span> |
| <span data-ttu-id="86ad7-124">displayName</span><span class="sxs-lookup"><span data-stu-id="86ad7-124">displayName</span></span>    | <span data-ttu-id="86ad7-125">String</span><span class="sxs-lookup"><span data-stu-id="86ad7-125">String</span></span>                                            | <span data-ttu-id="86ad7-126">会議室一覧に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="86ad7-126">The name associated with the room list.</span></span> |
| <span data-ttu-id="86ad7-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="86ad7-127">emailAddress</span></span>   | <span data-ttu-id="86ad7-128">String</span><span class="sxs-lookup"><span data-stu-id="86ad7-128">String</span></span>                                            | <span data-ttu-id="86ad7-129">会議室一覧の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="86ad7-129">The email address of the room list.</span></span> |
| <span data-ttu-id="86ad7-130">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="86ad7-130">geoCoordinates</span></span> | [<span data-ttu-id="86ad7-131">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="86ad7-131">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="86ad7-132">緯度、経度、および (オプションで) 高度座標での roomlist の位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="86ad7-132">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="86ad7-133">id</span><span class="sxs-lookup"><span data-stu-id="86ad7-133">id</span></span>             | <span data-ttu-id="86ad7-134">文字列</span><span class="sxs-lookup"><span data-stu-id="86ad7-134">String</span></span>                                            | <span data-ttu-id="86ad7-135">会議室一覧の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="86ad7-135">Unique identifier for the room list.</span></span> <span data-ttu-id="86ad7-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="86ad7-136">Read-only.</span></span> |
| <span data-ttu-id="86ad7-137">phone</span><span class="sxs-lookup"><span data-stu-id="86ad7-137">phone</span></span>          | <span data-ttu-id="86ad7-138">String</span><span class="sxs-lookup"><span data-stu-id="86ad7-138">String</span></span>                                            | <span data-ttu-id="86ad7-139">会議室一覧の電話番号。</span><span class="sxs-lookup"><span data-stu-id="86ad7-139">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="86ad7-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86ad7-140">Relationships</span></span>

| <span data-ttu-id="86ad7-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86ad7-141">Relationship</span></span> | <span data-ttu-id="86ad7-142">型</span><span class="sxs-lookup"><span data-stu-id="86ad7-142">Type</span></span>                         | <span data-ttu-id="86ad7-143">説明</span><span class="sxs-lookup"><span data-stu-id="86ad7-143">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="86ad7-144">ルーム</span><span class="sxs-lookup"><span data-stu-id="86ad7-144">rooms</span></span>        | <span data-ttu-id="86ad7-145">コレクションを[配置](place.md)する</span><span class="sxs-lookup"><span data-stu-id="86ad7-145">[place](place.md) collection</span></span> | <span data-ttu-id="86ad7-p103">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="86ad7-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86ad7-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86ad7-148">JSON representation</span></span>

<span data-ttu-id="86ad7-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86ad7-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

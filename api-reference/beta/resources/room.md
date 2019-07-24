---
title: room リソースの種類
description: テナント内のルームのプロパティを指定します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41c87daa31feda2907abab6f5711b4b88963095b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841291"
---
# <a name="room-resource-type"></a><span data-ttu-id="3eb89-103">room リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3eb89-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eb89-104">テナント内のルームを表します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="3eb89-105">Exchange Online では、各会議室が会議室メールボックスに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="3eb89-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="3eb89-106">派生元[](place.md)。</span><span class="sxs-lookup"><span data-stu-id="3eb89-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3eb89-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3eb89-107">Methods</span></span>

| <span data-ttu-id="3eb89-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3eb89-108">Method</span></span>                              | <span data-ttu-id="3eb89-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3eb89-109">Return Type</span></span>                  | <span data-ttu-id="3eb89-110">説明</span><span class="sxs-lookup"><span data-stu-id="3eb89-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="3eb89-111">プレースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3eb89-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="3eb89-112">要求された派生型のコレクション。 [](place.md)</span><span class="sxs-lookup"><span data-stu-id="3eb89-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="3eb89-113">テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="3eb89-114">たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。</span><span class="sxs-lookup"><span data-stu-id="3eb89-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="3eb89-115">場所を取得する</span><span class="sxs-lookup"><span data-stu-id="3eb89-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="3eb89-116">要求された派生型[](place.md)</span><span class="sxs-lookup"><span data-stu-id="3eb89-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="3eb89-117">ルームなど、指定された**place**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="3eb89-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eb89-118">Properties</span></span>

| <span data-ttu-id="3eb89-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eb89-119">Property</span></span>               | <span data-ttu-id="3eb89-120">型</span><span class="sxs-lookup"><span data-stu-id="3eb89-120">Type</span></span>                                              | <span data-ttu-id="3eb89-121">説明</span><span class="sxs-lookup"><span data-stu-id="3eb89-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="3eb89-122">address</span><span class="sxs-lookup"><span data-stu-id="3eb89-122">address</span></span>                | [<span data-ttu-id="3eb89-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3eb89-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="3eb89-124">会議室の住所。</span><span class="sxs-lookup"><span data-stu-id="3eb89-124">The street address of the room.</span></span> |
| <span data-ttu-id="3eb89-125">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="3eb89-125">audioDeviceName</span></span>        | <span data-ttu-id="3eb89-126">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-126">String</span></span>                                            | <span data-ttu-id="3eb89-127">ルーム内のオーディオデバイスの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="3eb89-128">bookingType</span><span class="sxs-lookup"><span data-stu-id="3eb89-128">bookingType</span></span>            | [<span data-ttu-id="3eb89-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="3eb89-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="3eb89-130">部屋の種類。</span><span class="sxs-lookup"><span data-stu-id="3eb89-130">Type of room.</span></span> <span data-ttu-id="3eb89-131">可能な値は、`standard`、`managed`、`reserved` です。</span><span class="sxs-lookup"><span data-stu-id="3eb89-131">Possible values are `standard`, `managed`, and `reserved`.</span></span> |
| <span data-ttu-id="3eb89-132">セキュリティ</span><span class="sxs-lookup"><span data-stu-id="3eb89-132">building</span></span>               | <span data-ttu-id="3eb89-133">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-133">String</span></span>                                            | <span data-ttu-id="3eb89-134">部屋がある建物名または建物番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="3eb89-135">最大</span><span class="sxs-lookup"><span data-stu-id="3eb89-135">capacity</span></span>               | <span data-ttu-id="3eb89-136">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-136">String</span></span>                                            | <span data-ttu-id="3eb89-137">会議室の容量を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="3eb89-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb89-138">displayName</span></span>            | <span data-ttu-id="3eb89-139">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-139">String</span></span>                                            | <span data-ttu-id="3eb89-140">ルームに関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="3eb89-140">The name associated with the room.</span></span> |
| <span data-ttu-id="3eb89-141">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="3eb89-141">displayDeviceName</span></span>      | <span data-ttu-id="3eb89-142">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-142">String</span></span>                                            | <span data-ttu-id="3eb89-143">ルームの表示デバイスの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="3eb89-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3eb89-144">emailAddress</span></span>           | <span data-ttu-id="3eb89-145">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-145">String</span></span>                                            | <span data-ttu-id="3eb89-146">会議室の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="3eb89-146">Email address of the room.</span></span> |
| <span data-ttu-id="3eb89-147">floorNumber</span><span class="sxs-lookup"><span data-stu-id="3eb89-147">floorNumber</span></span>            | <span data-ttu-id="3eb89-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb89-148">Int32</span></span>                                             | <span data-ttu-id="3eb89-149">部屋があるフロア番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-149">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="3eb89-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3eb89-150">geoCoordinates</span></span>         | [<span data-ttu-id="3eb89-151">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3eb89-151">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="3eb89-152">緯度、経度、および必要に応じて高度な座標での部屋の位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-152">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="3eb89-153">id</span><span class="sxs-lookup"><span data-stu-id="3eb89-153">id</span></span>                     | <span data-ttu-id="3eb89-154">文字列</span><span class="sxs-lookup"><span data-stu-id="3eb89-154">String</span></span>                                            | <span data-ttu-id="3eb89-155">ルームの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3eb89-155">Unique identifier for the room.</span></span> <span data-ttu-id="3eb89-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3eb89-156">Read-only.</span></span> |
| <span data-ttu-id="3eb89-157">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="3eb89-157">isWheelchairAccessible</span></span> | <span data-ttu-id="3eb89-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eb89-158">Boolean</span></span>                                           | <span data-ttu-id="3eb89-159">会議室に wheelchair アクセス可能かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-159">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="3eb89-160">label</span><span class="sxs-lookup"><span data-stu-id="3eb89-160">label</span></span>                  | <span data-ttu-id="3eb89-161">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-161">String</span></span>                                            | <span data-ttu-id="3eb89-162">ルームの内容を示すラベル (たとえば、数字または名前) を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-162">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="3eb89-163">ニックネーム</span><span class="sxs-lookup"><span data-stu-id="3eb89-163">nickname</span></span>               | <span data-ttu-id="3eb89-164">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-164">String</span></span>                                            | <span data-ttu-id="3eb89-165">会議室のニックネームを指定します (例: "conf room")。</span><span class="sxs-lookup"><span data-stu-id="3eb89-165">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="3eb89-166">phone</span><span class="sxs-lookup"><span data-stu-id="3eb89-166">phone</span></span>                  | <span data-ttu-id="3eb89-167">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-167">String</span></span>                                            | <span data-ttu-id="3eb89-168">会議室の電話番号。</span><span class="sxs-lookup"><span data-stu-id="3eb89-168">The phone number of the room.</span></span> |
| <span data-ttu-id="3eb89-169">タグ</span><span class="sxs-lookup"><span data-stu-id="3eb89-169">tags</span></span>                   | <span data-ttu-id="3eb89-170">String collection</span><span class="sxs-lookup"><span data-stu-id="3eb89-170">String collection</span></span>                                 | <span data-ttu-id="3eb89-171">ルームの追加機能を指定します。たとえば、ビューや家具の種類などの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="3eb89-171">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="3eb89-172">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="3eb89-172">videoDeviceName</span></span>        | <span data-ttu-id="3eb89-173">String</span><span class="sxs-lookup"><span data-stu-id="3eb89-173">String</span></span>                                            | <span data-ttu-id="3eb89-174">ルーム内のビデオデバイスの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-174">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="3eb89-175">bookingType の値</span><span class="sxs-lookup"><span data-stu-id="3eb89-175">bookingType values</span></span>

| <span data-ttu-id="3eb89-176">値</span><span class="sxs-lookup"><span data-stu-id="3eb89-176">Value</span></span>    | <span data-ttu-id="3eb89-177">説明</span><span class="sxs-lookup"><span data-stu-id="3eb89-177">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="3eb89-178">standard</span><span class="sxs-lookup"><span data-stu-id="3eb89-178">standard</span></span> | <span data-ttu-id="3eb89-179">このコマンドレットの他の設定に基づいて、会議室を予約することができます。</span><span class="sxs-lookup"><span data-stu-id="3eb89-179">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="3eb89-180">所有者、作成者、サイト所有者は引き続き対象アイテムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3eb89-180">This is the default value.</span></span> |
| <span data-ttu-id="3eb89-181">対象</span><span class="sxs-lookup"><span data-stu-id="3eb89-181">managed</span></span>  | <span data-ttu-id="3eb89-182">会議室が代理人によって管理されている</span><span class="sxs-lookup"><span data-stu-id="3eb89-182">The room is managed by a delegate</span></span>                         |
| <span data-ttu-id="3eb89-183">予約語</span><span class="sxs-lookup"><span data-stu-id="3eb89-183">reserved</span></span> | <span data-ttu-id="3eb89-184">ルームは、最初に提供された最初の提供元でのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="3eb89-184">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="3eb89-185">予約することはできません。</span><span class="sxs-lookup"><span data-stu-id="3eb89-185">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3eb89-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3eb89-186">Relationships</span></span>

<span data-ttu-id="3eb89-187">なし。</span><span class="sxs-lookup"><span data-stu-id="3eb89-187">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3eb89-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3eb89-188">JSON representation</span></span>

<span data-ttu-id="3eb89-189">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3eb89-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

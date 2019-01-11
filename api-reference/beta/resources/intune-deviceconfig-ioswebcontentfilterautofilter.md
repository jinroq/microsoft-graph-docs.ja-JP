---
title: iosWebContentFilterAutoFilter リソースの種類
description: IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。 構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。
localization_priority: Normal
ms.openlocfilehash: 02576565ecf764d33312477531d6a76c61911cb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868132"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="79d87-104">iosWebContentFilterAutoFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79d87-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="79d87-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79d87-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79d87-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79d87-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79d87-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79d87-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79d87-108">IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="79d87-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="79d87-109">構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。</span><span class="sxs-lookup"><span data-stu-id="79d87-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="79d87-110">[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="79d87-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79d87-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79d87-111">Properties</span></span>
|<span data-ttu-id="79d87-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79d87-112">Property</span></span>|<span data-ttu-id="79d87-113">種類</span><span class="sxs-lookup"><span data-stu-id="79d87-113">Type</span></span>|<span data-ttu-id="79d87-114">説明</span><span class="sxs-lookup"><span data-stu-id="79d87-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d87-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="79d87-115">allowedUrls</span></span>|<span data-ttu-id="79d87-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="79d87-116">String collection</span></span>|<span data-ttu-id="79d87-117">追加の Url のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="79d87-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="79d87-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="79d87-118">blockedUrls</span></span>|<span data-ttu-id="79d87-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="79d87-119">String collection</span></span>|<span data-ttu-id="79d87-120">追加の Url アクセスのブロック</span><span class="sxs-lookup"><span data-stu-id="79d87-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="79d87-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79d87-121">Relationships</span></span>
<span data-ttu-id="79d87-122">なし</span><span class="sxs-lookup"><span data-stu-id="79d87-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79d87-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79d87-123">JSON Representation</span></span>
<span data-ttu-id="79d87-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79d87-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```






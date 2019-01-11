---
title: adminConsent リソースの種類
description: 同意の情報を管理します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b6b2d9a8c32c9a1ce7e8587ebe853f7646b703a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815588"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="c6259-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6259-103">adminConsent resource type</span></span>

> <span data-ttu-id="c6259-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c6259-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6259-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6259-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6259-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6259-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6259-107">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="c6259-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="c6259-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6259-108">Properties</span></span>
|<span data-ttu-id="c6259-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6259-109">Property</span></span>|<span data-ttu-id="c6259-110">種類</span><span class="sxs-lookup"><span data-stu-id="c6259-110">Type</span></span>|<span data-ttu-id="c6259-111">説明</span><span class="sxs-lookup"><span data-stu-id="c6259-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6259-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="c6259-112">shareAPNSData</span></span>|[<span data-ttu-id="c6259-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="c6259-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="c6259-114">ユーザーと apple のデバイスのデータを共有するための管理者の同意の状態です。</span><span class="sxs-lookup"><span data-stu-id="c6259-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="c6259-115">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="c6259-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6259-116">関係</span><span class="sxs-lookup"><span data-stu-id="c6259-116">Relationships</span></span>
<span data-ttu-id="c6259-117">なし</span><span class="sxs-lookup"><span data-stu-id="c6259-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6259-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6259-118">JSON Representation</span></span>
<span data-ttu-id="c6259-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6259-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```






---
title: adminConsent リソースの種類
description: 同意の情報を管理します。
ms.openlocfilehash: da7197c995d9c87ab69db11ae0c6c0804482877d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071296"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="68995-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68995-103">adminConsent resource type</span></span>

> <span data-ttu-id="68995-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68995-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68995-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68995-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68995-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68995-107">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="68995-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="68995-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68995-108">Properties</span></span>
|<span data-ttu-id="68995-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68995-109">Property</span></span>|<span data-ttu-id="68995-110">型</span><span class="sxs-lookup"><span data-stu-id="68995-110">Type</span></span>|<span data-ttu-id="68995-111">説明</span><span class="sxs-lookup"><span data-stu-id="68995-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68995-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="68995-112">shareAPNSData</span></span>|[<span data-ttu-id="68995-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="68995-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="68995-114">ユーザーと apple のデバイスのデータを共有するための管理者の同意の状態です。</span><span class="sxs-lookup"><span data-stu-id="68995-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="68995-115">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="68995-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68995-116">関係</span><span class="sxs-lookup"><span data-stu-id="68995-116">Relationships</span></span>
<span data-ttu-id="68995-117">なし</span><span class="sxs-lookup"><span data-stu-id="68995-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68995-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68995-118">JSON Representation</span></span>
<span data-ttu-id="68995-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68995-119">Here is a JSON representation of the resource.</span></span>
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






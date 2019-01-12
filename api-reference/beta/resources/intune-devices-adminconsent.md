---
title: adminConsent リソースの種類
description: 同意の情報を管理します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 428729ff9a8a8ee5deb64c537922cb7a0417ba2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962129"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="d0208-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0208-103">adminConsent resource type</span></span>

> <span data-ttu-id="d0208-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0208-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0208-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0208-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0208-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0208-107">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="d0208-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="d0208-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0208-108">Properties</span></span>
|<span data-ttu-id="d0208-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0208-109">Property</span></span>|<span data-ttu-id="d0208-110">種類</span><span class="sxs-lookup"><span data-stu-id="d0208-110">Type</span></span>|<span data-ttu-id="d0208-111">説明</span><span class="sxs-lookup"><span data-stu-id="d0208-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0208-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="d0208-112">shareAPNSData</span></span>|[<span data-ttu-id="d0208-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="d0208-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="d0208-114">ユーザーと apple のデバイスのデータを共有するための管理者の同意の状態です。</span><span class="sxs-lookup"><span data-stu-id="d0208-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="d0208-115">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="d0208-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0208-116">関係</span><span class="sxs-lookup"><span data-stu-id="d0208-116">Relationships</span></span>
<span data-ttu-id="d0208-117">なし</span><span class="sxs-lookup"><span data-stu-id="d0208-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0208-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0208-118">JSON Representation</span></span>
<span data-ttu-id="d0208-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0208-119">Here is a JSON representation of the resource.</span></span>
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






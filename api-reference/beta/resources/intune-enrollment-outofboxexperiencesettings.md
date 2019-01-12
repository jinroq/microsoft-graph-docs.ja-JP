---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 70f1fb573409a55dd1e586b8e88133c5535de894
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977291"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="5a461-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a461-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="5a461-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a461-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a461-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a461-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a461-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a461-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a461-107">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="5a461-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="5a461-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a461-108">Properties</span></span>
|<span data-ttu-id="5a461-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a461-109">Property</span></span>|<span data-ttu-id="5a461-110">型</span><span class="sxs-lookup"><span data-stu-id="5a461-110">Type</span></span>|<span data-ttu-id="5a461-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a461-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a461-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="5a461-112">hidePrivacySettings</span></span>|<span data-ttu-id="5a461-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a461-113">Boolean</span></span>|<span data-ttu-id="5a461-114">ユーザーのプライバシー設定の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="5a461-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="5a461-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="5a461-115">hideEULA</span></span>|<span data-ttu-id="5a461-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a461-116">Boolean</span></span>|<span data-ttu-id="5a461-117">ユーザーに使用許諾契約書の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="5a461-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="5a461-118">userType</span><span class="sxs-lookup"><span data-stu-id="5a461-118">userType</span></span>|[<span data-ttu-id="5a461-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="5a461-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="5a461-120">ユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="5a461-120">Type of user.</span></span> <span data-ttu-id="5a461-121">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="5a461-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="5a461-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="5a461-122">deviceUsageType</span></span>|[<span data-ttu-id="5a461-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="5a461-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="5a461-124">AAD の結合の認証の種類です。</span><span class="sxs-lookup"><span data-stu-id="5a461-124">AAD join authentication type.</span></span> <span data-ttu-id="5a461-125">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="5a461-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="5a461-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="5a461-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="5a461-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a461-127">Boolean</span></span>|<span data-ttu-id="5a461-128">かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合</span><span class="sxs-lookup"><span data-stu-id="5a461-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="5a461-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="5a461-129">hideEscapeLink</span></span>|<span data-ttu-id="5a461-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a461-130">Boolean</span></span>|<span data-ttu-id="5a461-131">ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合</span><span class="sxs-lookup"><span data-stu-id="5a461-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a461-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a461-132">Relationships</span></span>
<span data-ttu-id="5a461-133">なし</span><span class="sxs-lookup"><span data-stu-id="5a461-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a461-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a461-134">JSON Representation</span></span>
<span data-ttu-id="5a461-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a461-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```






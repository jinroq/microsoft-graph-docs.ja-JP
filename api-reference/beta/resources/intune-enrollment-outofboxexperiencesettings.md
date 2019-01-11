---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af276dd520df9ee3b257650e703813de355bed9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882734"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="24769-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24769-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="24769-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24769-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24769-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24769-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24769-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24769-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24769-107">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="24769-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="24769-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24769-108">Properties</span></span>
|<span data-ttu-id="24769-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24769-109">Property</span></span>|<span data-ttu-id="24769-110">種類</span><span class="sxs-lookup"><span data-stu-id="24769-110">Type</span></span>|<span data-ttu-id="24769-111">説明</span><span class="sxs-lookup"><span data-stu-id="24769-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24769-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="24769-112">hidePrivacySettings</span></span>|<span data-ttu-id="24769-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="24769-113">Boolean</span></span>|<span data-ttu-id="24769-114">ユーザーのプライバシー設定の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="24769-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="24769-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="24769-115">hideEULA</span></span>|<span data-ttu-id="24769-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="24769-116">Boolean</span></span>|<span data-ttu-id="24769-117">ユーザーに使用許諾契約書の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="24769-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="24769-118">userType</span><span class="sxs-lookup"><span data-stu-id="24769-118">userType</span></span>|[<span data-ttu-id="24769-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="24769-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="24769-120">ユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="24769-120">Type of user.</span></span> <span data-ttu-id="24769-121">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="24769-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="24769-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="24769-122">deviceUsageType</span></span>|[<span data-ttu-id="24769-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="24769-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="24769-124">AAD の結合の認証の種類です。</span><span class="sxs-lookup"><span data-stu-id="24769-124">AAD join authentication type.</span></span> <span data-ttu-id="24769-125">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="24769-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="24769-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="24769-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="24769-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="24769-127">Boolean</span></span>|<span data-ttu-id="24769-128">かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合</span><span class="sxs-lookup"><span data-stu-id="24769-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="24769-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="24769-129">hideEscapeLink</span></span>|<span data-ttu-id="24769-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="24769-130">Boolean</span></span>|<span data-ttu-id="24769-131">ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合</span><span class="sxs-lookup"><span data-stu-id="24769-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="24769-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24769-132">Relationships</span></span>
<span data-ttu-id="24769-133">なし</span><span class="sxs-lookup"><span data-stu-id="24769-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24769-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24769-134">JSON Representation</span></span>
<span data-ttu-id="24769-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24769-135">Here is a JSON representation of the resource.</span></span>
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






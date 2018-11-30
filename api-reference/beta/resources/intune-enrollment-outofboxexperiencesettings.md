---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
ms.openlocfilehash: 7d685c7e229828309e2ee759396215c3cd8dfac9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073866"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="43bdc-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43bdc-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="43bdc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43bdc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43bdc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43bdc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="43bdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43bdc-107">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="43bdc-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="43bdc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43bdc-108">Properties</span></span>
|<span data-ttu-id="43bdc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43bdc-109">Property</span></span>|<span data-ttu-id="43bdc-110">型</span><span class="sxs-lookup"><span data-stu-id="43bdc-110">Type</span></span>|<span data-ttu-id="43bdc-111">説明</span><span class="sxs-lookup"><span data-stu-id="43bdc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43bdc-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="43bdc-112">hidePrivacySettings</span></span>|<span data-ttu-id="43bdc-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="43bdc-113">Boolean</span></span>|<span data-ttu-id="43bdc-114">ユーザーのプライバシー設定の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="43bdc-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="43bdc-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="43bdc-115">hideEULA</span></span>|<span data-ttu-id="43bdc-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="43bdc-116">Boolean</span></span>|<span data-ttu-id="43bdc-117">ユーザーに使用許諾契約書の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="43bdc-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="43bdc-118">userType</span><span class="sxs-lookup"><span data-stu-id="43bdc-118">userType</span></span>|[<span data-ttu-id="43bdc-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="43bdc-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="43bdc-120">ユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="43bdc-120">Type of user.</span></span> <span data-ttu-id="43bdc-121">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="43bdc-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="43bdc-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="43bdc-122">deviceUsageType</span></span>|[<span data-ttu-id="43bdc-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="43bdc-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="43bdc-124">AAD の結合の認証の種類です。</span><span class="sxs-lookup"><span data-stu-id="43bdc-124">AAD join authentication type.</span></span> <span data-ttu-id="43bdc-125">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="43bdc-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="43bdc-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="43bdc-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="43bdc-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="43bdc-127">Boolean</span></span>|<span data-ttu-id="43bdc-128">かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合</span><span class="sxs-lookup"><span data-stu-id="43bdc-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="43bdc-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="43bdc-129">hideEscapeLink</span></span>|<span data-ttu-id="43bdc-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="43bdc-130">Boolean</span></span>|<span data-ttu-id="43bdc-131">ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合</span><span class="sxs-lookup"><span data-stu-id="43bdc-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="43bdc-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43bdc-132">Relationships</span></span>
<span data-ttu-id="43bdc-133">なし</span><span class="sxs-lookup"><span data-stu-id="43bdc-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43bdc-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43bdc-134">JSON Representation</span></span>
<span data-ttu-id="43bdc-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43bdc-135">Here is a JSON representation of the resource.</span></span>
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






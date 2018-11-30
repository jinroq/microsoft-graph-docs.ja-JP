---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
ms.openlocfilehash: edb99b2fac02b95ebd2634749bdaa8d4acfec781
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070967"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="76239-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="76239-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="76239-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76239-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76239-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76239-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76239-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76239-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76239-107">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="76239-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76239-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="76239-108">Prerequisites</span></span>
<span data-ttu-id="76239-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76239-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76239-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76239-111">Permission type</span></span>|<span data-ttu-id="76239-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76239-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76239-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76239-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76239-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76239-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76239-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76239-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76239-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76239-116">Not supported.</span></span>|
|<span data-ttu-id="76239-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76239-117">Application</span></span>|<span data-ttu-id="76239-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76239-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76239-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76239-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76239-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76239-120">Request headers</span></span>
|<span data-ttu-id="76239-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76239-121">Header</span></span>|<span data-ttu-id="76239-122">値</span><span class="sxs-lookup"><span data-stu-id="76239-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76239-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76239-123">Authorization</span></span>|<span data-ttu-id="76239-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="76239-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76239-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76239-125">Accept</span></span>|<span data-ttu-id="76239-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76239-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76239-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="76239-127">Request body</span></span>
<span data-ttu-id="76239-128">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="76239-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="76239-129">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="76239-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="76239-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76239-130">Property</span></span>|<span data-ttu-id="76239-131">型</span><span class="sxs-lookup"><span data-stu-id="76239-131">Type</span></span>|<span data-ttu-id="76239-132">説明</span><span class="sxs-lookup"><span data-stu-id="76239-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76239-133">id</span><span class="sxs-lookup"><span data-stu-id="76239-133">id</span></span>|<span data-ttu-id="76239-134">String</span><span class="sxs-lookup"><span data-stu-id="76239-134">String</span></span>|<span data-ttu-id="76239-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="76239-135">Key of the entity.</span></span>|
|<span data-ttu-id="76239-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="76239-136">gracePeriodHours</span></span>|<span data-ttu-id="76239-137">Int32</span><span class="sxs-lookup"><span data-stu-id="76239-137">Int32</span></span>|<span data-ttu-id="76239-138">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="76239-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="76239-139">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="76239-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="76239-140">actionType</span><span class="sxs-lookup"><span data-stu-id="76239-140">actionType</span></span>|[<span data-ttu-id="76239-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="76239-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="76239-142">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="76239-142">What action to take.</span></span> <span data-ttu-id="76239-143">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="76239-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="76239-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="76239-144">notificationTemplateId</span></span>|<span data-ttu-id="76239-145">String</span><span class="sxs-lookup"><span data-stu-id="76239-145">String</span></span>|<span data-ttu-id="76239-146">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="76239-146">What notification Message template to use</span></span>|
|<span data-ttu-id="76239-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="76239-147">notificationMessageCCList</span></span>|<span data-ttu-id="76239-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="76239-148">String collection</span></span>|<span data-ttu-id="76239-149">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="76239-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="76239-150">応答</span><span class="sxs-lookup"><span data-stu-id="76239-150">Response</span></span>
<span data-ttu-id="76239-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76239-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76239-152">例</span><span class="sxs-lookup"><span data-stu-id="76239-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="76239-153">要求</span><span class="sxs-lookup"><span data-stu-id="76239-153">Request</span></span>
<span data-ttu-id="76239-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76239-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="76239-155">応答</span><span class="sxs-lookup"><span data-stu-id="76239-155">Response</span></span>
<span data-ttu-id="76239-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76239-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```






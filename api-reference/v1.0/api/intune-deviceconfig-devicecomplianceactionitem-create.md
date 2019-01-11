---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b2102b0242c002c57747ebecf1731fdb325e898
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871009"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="47b6e-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="47b6e-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="47b6e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47b6e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47b6e-105">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="47b6e-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47b6e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="47b6e-106">Prerequisites</span></span>
<span data-ttu-id="47b6e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b6e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47b6e-109">Permission type</span></span>|<span data-ttu-id="47b6e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47b6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47b6e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47b6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47b6e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b6e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47b6e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47b6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47b6e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47b6e-114">Not supported.</span></span>|
|<span data-ttu-id="47b6e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47b6e-115">Application</span></span>|<span data-ttu-id="47b6e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47b6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47b6e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47b6e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47b6e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47b6e-118">Request headers</span></span>
|<span data-ttu-id="47b6e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47b6e-119">Header</span></span>|<span data-ttu-id="47b6e-120">値</span><span class="sxs-lookup"><span data-stu-id="47b6e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47b6e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47b6e-121">Authorization</span></span>|<span data-ttu-id="47b6e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="47b6e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47b6e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="47b6e-123">Accept</span></span>|<span data-ttu-id="47b6e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47b6e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b6e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="47b6e-125">Request body</span></span>
<span data-ttu-id="47b6e-126">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="47b6e-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="47b6e-127">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="47b6e-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="47b6e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47b6e-128">Property</span></span>|<span data-ttu-id="47b6e-129">種類</span><span class="sxs-lookup"><span data-stu-id="47b6e-129">Type</span></span>|<span data-ttu-id="47b6e-130">説明</span><span class="sxs-lookup"><span data-stu-id="47b6e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47b6e-131">ID</span><span class="sxs-lookup"><span data-stu-id="47b6e-131">id</span></span>|<span data-ttu-id="47b6e-132">String</span><span class="sxs-lookup"><span data-stu-id="47b6e-132">String</span></span>|<span data-ttu-id="47b6e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47b6e-133">Key of the entity.</span></span>|
|<span data-ttu-id="47b6e-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="47b6e-134">gracePeriodHours</span></span>|<span data-ttu-id="47b6e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="47b6e-135">Int32</span></span>|<span data-ttu-id="47b6e-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="47b6e-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="47b6e-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="47b6e-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="47b6e-138">actionType</span><span class="sxs-lookup"><span data-stu-id="47b6e-138">actionType</span></span>|[<span data-ttu-id="47b6e-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="47b6e-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="47b6e-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="47b6e-140">What action to take.</span></span> <span data-ttu-id="47b6e-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="47b6e-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="47b6e-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="47b6e-142">notificationTemplateId</span></span>|<span data-ttu-id="47b6e-143">String</span><span class="sxs-lookup"><span data-stu-id="47b6e-143">String</span></span>|<span data-ttu-id="47b6e-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="47b6e-144">What notification Message template to use</span></span>|
|<span data-ttu-id="47b6e-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="47b6e-145">notificationMessageCCList</span></span>|<span data-ttu-id="47b6e-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="47b6e-146">String collection</span></span>|<span data-ttu-id="47b6e-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="47b6e-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="47b6e-148">応答</span><span class="sxs-lookup"><span data-stu-id="47b6e-148">Response</span></span>
<span data-ttu-id="47b6e-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="47b6e-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b6e-150">例</span><span class="sxs-lookup"><span data-stu-id="47b6e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="47b6e-151">要求</span><span class="sxs-lookup"><span data-stu-id="47b6e-151">Request</span></span>
<span data-ttu-id="47b6e-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47b6e-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="47b6e-153">応答</span><span class="sxs-lookup"><span data-stu-id="47b6e-153">Response</span></span>
<span data-ttu-id="47b6e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47b6e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




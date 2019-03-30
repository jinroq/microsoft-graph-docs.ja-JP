---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dca5374dcb75e93667454389f0104861bb9f1d7c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988148"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="0cd20-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="0cd20-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="0cd20-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cd20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd20-105">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0cd20-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd20-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0cd20-106">Prerequisites</span></span>
<span data-ttu-id="0cd20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cd20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd20-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cd20-109">Permission type</span></span>|<span data-ttu-id="0cd20-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cd20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd20-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd20-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd20-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cd20-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd20-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd20-114">Not supported.</span></span>|
|<span data-ttu-id="0cd20-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cd20-115">Application</span></span>|<span data-ttu-id="0cd20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd20-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cd20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0cd20-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cd20-118">Request headers</span></span>
|<span data-ttu-id="0cd20-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cd20-119">Header</span></span>|<span data-ttu-id="0cd20-120">値</span><span class="sxs-lookup"><span data-stu-id="0cd20-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd20-121">Authorization</span></span>|<span data-ttu-id="0cd20-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cd20-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd20-123">承諾</span><span class="sxs-lookup"><span data-stu-id="0cd20-123">Accept</span></span>|<span data-ttu-id="0cd20-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd20-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd20-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cd20-125">Request body</span></span>
<span data-ttu-id="0cd20-126">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cd20-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="0cd20-127">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0cd20-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="0cd20-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd20-128">Property</span></span>|<span data-ttu-id="0cd20-129">型</span><span class="sxs-lookup"><span data-stu-id="0cd20-129">Type</span></span>|<span data-ttu-id="0cd20-130">説明</span><span class="sxs-lookup"><span data-stu-id="0cd20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd20-131">id</span><span class="sxs-lookup"><span data-stu-id="0cd20-131">id</span></span>|<span data-ttu-id="0cd20-132">String</span><span class="sxs-lookup"><span data-stu-id="0cd20-132">String</span></span>|<span data-ttu-id="0cd20-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0cd20-133">Key of the entity.</span></span>|
|<span data-ttu-id="0cd20-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="0cd20-134">gracePeriodHours</span></span>|<span data-ttu-id="0cd20-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd20-135">Int32</span></span>|<span data-ttu-id="0cd20-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="0cd20-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="0cd20-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="0cd20-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="0cd20-138">actionType</span><span class="sxs-lookup"><span data-stu-id="0cd20-138">actionType</span></span>|[<span data-ttu-id="0cd20-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="0cd20-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="0cd20-140">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="0cd20-140">What action to take.</span></span> <span data-ttu-id="0cd20-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="0cd20-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="0cd20-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="0cd20-142">notificationTemplateId</span></span>|<span data-ttu-id="0cd20-143">String</span><span class="sxs-lookup"><span data-stu-id="0cd20-143">String</span></span>|<span data-ttu-id="0cd20-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="0cd20-144">What notification Message template to use</span></span>|
|<span data-ttu-id="0cd20-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="0cd20-145">notificationMessageCCList</span></span>|<span data-ttu-id="0cd20-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd20-146">String collection</span></span>|<span data-ttu-id="0cd20-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="0cd20-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="0cd20-148">応答</span><span class="sxs-lookup"><span data-stu-id="0cd20-148">Response</span></span>
<span data-ttu-id="0cd20-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0cd20-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd20-150">例</span><span class="sxs-lookup"><span data-stu-id="0cd20-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd20-151">要求</span><span class="sxs-lookup"><span data-stu-id="0cd20-151">Request</span></span>
<span data-ttu-id="0cd20-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cd20-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0cd20-153">応答</span><span class="sxs-lookup"><span data-stu-id="0cd20-153">Response</span></span>
<span data-ttu-id="0cd20-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cd20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




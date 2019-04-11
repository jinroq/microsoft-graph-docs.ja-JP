---
title: deviceComplianceActionItem の更新
description: deviceComplianceActionItem オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 497a5e8b653d7873a45a242d0594d025f5e8a680
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799203"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="e5566-103">deviceComplianceActionItem の更新</span><span class="sxs-lookup"><span data-stu-id="e5566-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="e5566-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5566-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5566-106">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5566-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5566-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5566-107">Prerequisites</span></span>
<span data-ttu-id="e5566-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5566-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5566-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5566-110">Permission type</span></span>|<span data-ttu-id="e5566-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5566-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5566-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5566-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5566-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5566-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5566-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5566-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5566-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5566-115">Not supported.</span></span>|
|<span data-ttu-id="e5566-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5566-116">Application</span></span>|<span data-ttu-id="e5566-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5566-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5566-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5566-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="e5566-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5566-119">Request headers</span></span>
|<span data-ttu-id="e5566-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5566-120">Header</span></span>|<span data-ttu-id="e5566-121">値</span><span class="sxs-lookup"><span data-stu-id="e5566-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5566-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5566-122">Authorization</span></span>|<span data-ttu-id="e5566-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5566-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5566-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e5566-124">Accept</span></span>|<span data-ttu-id="e5566-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5566-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5566-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5566-126">Request body</span></span>
<span data-ttu-id="e5566-127">要求本文で、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5566-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="e5566-128">次の表に、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e5566-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="e5566-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5566-129">Property</span></span>|<span data-ttu-id="e5566-130">型</span><span class="sxs-lookup"><span data-stu-id="e5566-130">Type</span></span>|<span data-ttu-id="e5566-131">説明</span><span class="sxs-lookup"><span data-stu-id="e5566-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5566-132">id</span><span class="sxs-lookup"><span data-stu-id="e5566-132">id</span></span>|<span data-ttu-id="e5566-133">String</span><span class="sxs-lookup"><span data-stu-id="e5566-133">String</span></span>|<span data-ttu-id="e5566-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5566-134">Key of the entity.</span></span>|
|<span data-ttu-id="e5566-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="e5566-135">gracePeriodHours</span></span>|<span data-ttu-id="e5566-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e5566-136">Int32</span></span>|<span data-ttu-id="e5566-137">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="e5566-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="e5566-138">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="e5566-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="e5566-139">actionType</span><span class="sxs-lookup"><span data-stu-id="e5566-139">actionType</span></span>|[<span data-ttu-id="e5566-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="e5566-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="e5566-141">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="e5566-141">What action to take.</span></span> <span data-ttu-id="e5566-142">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="e5566-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="e5566-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="e5566-143">notificationTemplateId</span></span>|<span data-ttu-id="e5566-144">String</span><span class="sxs-lookup"><span data-stu-id="e5566-144">String</span></span>|<span data-ttu-id="e5566-145">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="e5566-145">What notification Message template to use</span></span>|
|<span data-ttu-id="e5566-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="e5566-146">notificationMessageCCList</span></span>|<span data-ttu-id="e5566-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e5566-147">String collection</span></span>|<span data-ttu-id="e5566-148">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="e5566-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="e5566-149">応答</span><span class="sxs-lookup"><span data-stu-id="e5566-149">Response</span></span>
<span data-ttu-id="e5566-150">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e5566-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5566-151">例</span><span class="sxs-lookup"><span data-stu-id="e5566-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5566-152">要求</span><span class="sxs-lookup"><span data-stu-id="e5566-152">Request</span></span>
<span data-ttu-id="e5566-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5566-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="e5566-154">応答</span><span class="sxs-lookup"><span data-stu-id="e5566-154">Response</span></span>
<span data-ttu-id="e5566-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5566-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






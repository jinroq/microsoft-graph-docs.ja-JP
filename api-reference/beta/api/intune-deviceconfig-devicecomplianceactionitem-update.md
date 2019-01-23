---
title: deviceComplianceActionItem の更新
description: deviceComplianceActionItem オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77f1292e240d8d8887adff98aa9326685659bb77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404975"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="09384-103">deviceComplianceActionItem の更新</span><span class="sxs-lookup"><span data-stu-id="09384-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="09384-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09384-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09384-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09384-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09384-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09384-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09384-107">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09384-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09384-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="09384-108">Prerequisites</span></span>
<span data-ttu-id="09384-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09384-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="09384-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09384-111">Permission type</span></span>|<span data-ttu-id="09384-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09384-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09384-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09384-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09384-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09384-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09384-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09384-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09384-116">Not supported.</span></span>|
|<span data-ttu-id="09384-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09384-117">Application</span></span>|<span data-ttu-id="09384-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09384-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09384-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09384-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="09384-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09384-120">Request headers</span></span>
|<span data-ttu-id="09384-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09384-121">Header</span></span>|<span data-ttu-id="09384-122">値</span><span class="sxs-lookup"><span data-stu-id="09384-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09384-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09384-123">Authorization</span></span>|<span data-ttu-id="09384-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="09384-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09384-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09384-125">Accept</span></span>|<span data-ttu-id="09384-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09384-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09384-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="09384-127">Request body</span></span>
<span data-ttu-id="09384-128">要求本文で、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09384-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="09384-129">次の表に、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09384-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="09384-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09384-130">Property</span></span>|<span data-ttu-id="09384-131">型</span><span class="sxs-lookup"><span data-stu-id="09384-131">Type</span></span>|<span data-ttu-id="09384-132">説明</span><span class="sxs-lookup"><span data-stu-id="09384-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09384-133">id</span><span class="sxs-lookup"><span data-stu-id="09384-133">id</span></span>|<span data-ttu-id="09384-134">String</span><span class="sxs-lookup"><span data-stu-id="09384-134">String</span></span>|<span data-ttu-id="09384-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09384-135">Key of the entity.</span></span>|
|<span data-ttu-id="09384-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="09384-136">gracePeriodHours</span></span>|<span data-ttu-id="09384-137">Int32</span><span class="sxs-lookup"><span data-stu-id="09384-137">Int32</span></span>|<span data-ttu-id="09384-138">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="09384-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="09384-139">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="09384-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="09384-140">actionType</span><span class="sxs-lookup"><span data-stu-id="09384-140">actionType</span></span>|[<span data-ttu-id="09384-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="09384-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="09384-142">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="09384-142">What action to take.</span></span> <span data-ttu-id="09384-143">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="09384-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="09384-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="09384-144">notificationTemplateId</span></span>|<span data-ttu-id="09384-145">String</span><span class="sxs-lookup"><span data-stu-id="09384-145">String</span></span>|<span data-ttu-id="09384-146">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="09384-146">What notification Message template to use</span></span>|
|<span data-ttu-id="09384-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="09384-147">notificationMessageCCList</span></span>|<span data-ttu-id="09384-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09384-148">String collection</span></span>|<span data-ttu-id="09384-149">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="09384-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="09384-150">応答</span><span class="sxs-lookup"><span data-stu-id="09384-150">Response</span></span>
<span data-ttu-id="09384-151">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="09384-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09384-152">例</span><span class="sxs-lookup"><span data-stu-id="09384-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="09384-153">要求</span><span class="sxs-lookup"><span data-stu-id="09384-153">Request</span></span>
<span data-ttu-id="09384-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09384-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09384-155">応答</span><span class="sxs-lookup"><span data-stu-id="09384-155">Response</span></span>
<span data-ttu-id="09384-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09384-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





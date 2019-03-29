---
title: auditEvent の作成
description: 新しい auditEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a11ca29ca4d251285ef4f6a1842b9d7174ee66f5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972684"
---
# <a name="create-auditevent"></a><span data-ttu-id="c82b6-103">auditEvent の作成</span><span class="sxs-lookup"><span data-stu-id="c82b6-103">Create auditEvent</span></span>

> <span data-ttu-id="c82b6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c82b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c82b6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c82b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c82b6-106">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c82b6-106">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c82b6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c82b6-107">Prerequisites</span></span>
<span data-ttu-id="c82b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c82b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c82b6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c82b6-110">Permission type</span></span>|<span data-ttu-id="c82b6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c82b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c82b6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c82b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c82b6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82b6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c82b6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c82b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c82b6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c82b6-115">Not supported.</span></span>|
|<span data-ttu-id="c82b6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c82b6-116">Application</span></span>|<span data-ttu-id="c82b6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c82b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c82b6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c82b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="c82b6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c82b6-119">Request headers</span></span>
|<span data-ttu-id="c82b6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c82b6-120">Header</span></span>|<span data-ttu-id="c82b6-121">値</span><span class="sxs-lookup"><span data-stu-id="c82b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c82b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c82b6-122">Authorization</span></span>|<span data-ttu-id="c82b6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c82b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c82b6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c82b6-124">Accept</span></span>|<span data-ttu-id="c82b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c82b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c82b6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c82b6-126">Request body</span></span>
<span data-ttu-id="c82b6-127">要求本文で、auditEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c82b6-127">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="c82b6-128">次の表に、auditEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c82b6-128">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="c82b6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c82b6-129">Property</span></span>|<span data-ttu-id="c82b6-130">型</span><span class="sxs-lookup"><span data-stu-id="c82b6-130">Type</span></span>|<span data-ttu-id="c82b6-131">説明</span><span class="sxs-lookup"><span data-stu-id="c82b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c82b6-132">id</span><span class="sxs-lookup"><span data-stu-id="c82b6-132">id</span></span>|<span data-ttu-id="c82b6-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c82b6-133">String</span></span>|<span data-ttu-id="c82b6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c82b6-134">Key of the entity.</span></span>|
|<span data-ttu-id="c82b6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c82b6-135">displayName</span></span>|<span data-ttu-id="c82b6-136">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-136">String</span></span>|<span data-ttu-id="c82b6-137">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="c82b6-137">Event display name.</span></span>|
|<span data-ttu-id="c82b6-138">componentName</span><span class="sxs-lookup"><span data-stu-id="c82b6-138">componentName</span></span>|<span data-ttu-id="c82b6-139">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-139">String</span></span>|<span data-ttu-id="c82b6-140">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="c82b6-140">Component name.</span></span>|
|<span data-ttu-id="c82b6-141">actor</span><span class="sxs-lookup"><span data-stu-id="c82b6-141">actor</span></span>|[<span data-ttu-id="c82b6-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="c82b6-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="c82b6-143">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="c82b6-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="c82b6-144">activity</span><span class="sxs-lookup"><span data-stu-id="c82b6-144">activity</span></span>|<span data-ttu-id="c82b6-145">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-145">String</span></span>|<span data-ttu-id="c82b6-146">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="c82b6-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="c82b6-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="c82b6-147">activityDateTime</span></span>|<span data-ttu-id="c82b6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c82b6-148">DateTimeOffset</span></span>|<span data-ttu-id="c82b6-149">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="c82b6-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="c82b6-150">activityType</span><span class="sxs-lookup"><span data-stu-id="c82b6-150">activityType</span></span>|<span data-ttu-id="c82b6-151">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-151">String</span></span>|<span data-ttu-id="c82b6-152">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="c82b6-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="c82b6-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="c82b6-153">activityOperationType</span></span>|<span data-ttu-id="c82b6-154">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-154">String</span></span>|<span data-ttu-id="c82b6-155">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="c82b6-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="c82b6-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="c82b6-156">activityResult</span></span>|<span data-ttu-id="c82b6-157">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-157">String</span></span>|<span data-ttu-id="c82b6-158">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="c82b6-158">The result of the activity.</span></span>|
|<span data-ttu-id="c82b6-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="c82b6-159">correlationId</span></span>|<span data-ttu-id="c82b6-160">Guid</span><span class="sxs-lookup"><span data-stu-id="c82b6-160">Guid</span></span>|<span data-ttu-id="c82b6-161">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="c82b6-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="c82b6-162">resources</span><span class="sxs-lookup"><span data-stu-id="c82b6-162">resources</span></span>|<span data-ttu-id="c82b6-163">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c82b6-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="c82b6-164">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="c82b6-164">Resources being modified.</span></span>|
|<span data-ttu-id="c82b6-165">category</span><span class="sxs-lookup"><span data-stu-id="c82b6-165">category</span></span>|<span data-ttu-id="c82b6-166">String</span><span class="sxs-lookup"><span data-stu-id="c82b6-166">String</span></span>|<span data-ttu-id="c82b6-167">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="c82b6-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="c82b6-168">応答</span><span class="sxs-lookup"><span data-stu-id="c82b6-168">Response</span></span>
<span data-ttu-id="c82b6-169">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c82b6-169">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c82b6-170">例</span><span class="sxs-lookup"><span data-stu-id="c82b6-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="c82b6-171">要求</span><span class="sxs-lookup"><span data-stu-id="c82b6-171">Request</span></span>
<span data-ttu-id="c82b6-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c82b6-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1390

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="c82b6-173">応答</span><span class="sxs-lookup"><span data-stu-id="c82b6-173">Response</span></span>
<span data-ttu-id="c82b6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c82b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```





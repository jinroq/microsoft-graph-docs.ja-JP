---
title: auditEvent の作成
description: 新しい auditEvent オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 0997ca2e9a7bf5421d20e2e3c784ebd444943d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318411"
---
# <a name="create-auditevent"></a><span data-ttu-id="236a0-103">auditEvent の作成</span><span class="sxs-lookup"><span data-stu-id="236a0-103">Create auditEvent</span></span>

> <span data-ttu-id="236a0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="236a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="236a0-105">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="236a0-105">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="236a0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="236a0-106">Prerequisites</span></span>
<span data-ttu-id="236a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="236a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="236a0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="236a0-109">Permission type</span></span>|<span data-ttu-id="236a0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="236a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="236a0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="236a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="236a0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="236a0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="236a0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="236a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="236a0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="236a0-114">Not supported.</span></span>|
|<span data-ttu-id="236a0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="236a0-115">Application</span></span>|<span data-ttu-id="236a0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="236a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="236a0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="236a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="236a0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="236a0-118">Request headers</span></span>
|<span data-ttu-id="236a0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="236a0-119">Header</span></span>|<span data-ttu-id="236a0-120">値</span><span class="sxs-lookup"><span data-stu-id="236a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="236a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="236a0-121">Authorization</span></span>|<span data-ttu-id="236a0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="236a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="236a0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="236a0-123">Accept</span></span>|<span data-ttu-id="236a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="236a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="236a0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="236a0-125">Request body</span></span>
<span data-ttu-id="236a0-126">要求本文で、auditEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="236a0-126">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="236a0-127">次の表に、auditEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="236a0-127">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="236a0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="236a0-128">Property</span></span>|<span data-ttu-id="236a0-129">種類</span><span class="sxs-lookup"><span data-stu-id="236a0-129">Type</span></span>|<span data-ttu-id="236a0-130">説明</span><span class="sxs-lookup"><span data-stu-id="236a0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="236a0-131">ID</span><span class="sxs-lookup"><span data-stu-id="236a0-131">id</span></span>|<span data-ttu-id="236a0-132">String</span><span class="sxs-lookup"><span data-stu-id="236a0-132">String</span></span>|<span data-ttu-id="236a0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="236a0-133">Key of the entity.</span></span>|
|<span data-ttu-id="236a0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="236a0-134">displayName</span></span>|<span data-ttu-id="236a0-135">String</span><span class="sxs-lookup"><span data-stu-id="236a0-135">String</span></span>|<span data-ttu-id="236a0-136">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="236a0-136">Event display name.</span></span>|
|<span data-ttu-id="236a0-137">componentName</span><span class="sxs-lookup"><span data-stu-id="236a0-137">componentName</span></span>|<span data-ttu-id="236a0-138">String</span><span class="sxs-lookup"><span data-stu-id="236a0-138">String</span></span>|<span data-ttu-id="236a0-139">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="236a0-139">Component name.</span></span>|
|<span data-ttu-id="236a0-140">actor</span><span class="sxs-lookup"><span data-stu-id="236a0-140">actor</span></span>|[<span data-ttu-id="236a0-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="236a0-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="236a0-142">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="236a0-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="236a0-143">activity</span><span class="sxs-lookup"><span data-stu-id="236a0-143">activity</span></span>|<span data-ttu-id="236a0-144">String</span><span class="sxs-lookup"><span data-stu-id="236a0-144">String</span></span>|<span data-ttu-id="236a0-145">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="236a0-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="236a0-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="236a0-146">activityDateTime</span></span>|<span data-ttu-id="236a0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236a0-147">DateTimeOffset</span></span>|<span data-ttu-id="236a0-148">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="236a0-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="236a0-149">activityType</span><span class="sxs-lookup"><span data-stu-id="236a0-149">activityType</span></span>|<span data-ttu-id="236a0-150">String</span><span class="sxs-lookup"><span data-stu-id="236a0-150">String</span></span>|<span data-ttu-id="236a0-151">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="236a0-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="236a0-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="236a0-152">activityOperationType</span></span>|<span data-ttu-id="236a0-153">String</span><span class="sxs-lookup"><span data-stu-id="236a0-153">String</span></span>|<span data-ttu-id="236a0-154">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="236a0-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="236a0-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="236a0-155">activityResult</span></span>|<span data-ttu-id="236a0-156">String</span><span class="sxs-lookup"><span data-stu-id="236a0-156">String</span></span>|<span data-ttu-id="236a0-157">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="236a0-157">The result of the activity.</span></span>|
|<span data-ttu-id="236a0-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="236a0-158">correlationId</span></span>|<span data-ttu-id="236a0-159">Guid</span><span class="sxs-lookup"><span data-stu-id="236a0-159">Guid</span></span>|<span data-ttu-id="236a0-160">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="236a0-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="236a0-161">resources</span><span class="sxs-lookup"><span data-stu-id="236a0-161">resources</span></span>|<span data-ttu-id="236a0-162">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="236a0-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="236a0-163">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="236a0-163">Resources being modified.</span></span>|
|<span data-ttu-id="236a0-164">category</span><span class="sxs-lookup"><span data-stu-id="236a0-164">category</span></span>|<span data-ttu-id="236a0-165">String</span><span class="sxs-lookup"><span data-stu-id="236a0-165">String</span></span>|<span data-ttu-id="236a0-166">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="236a0-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="236a0-167">応答</span><span class="sxs-lookup"><span data-stu-id="236a0-167">Response</span></span>
<span data-ttu-id="236a0-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="236a0-168">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="236a0-169">例</span><span class="sxs-lookup"><span data-stu-id="236a0-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="236a0-170">要求</span><span class="sxs-lookup"><span data-stu-id="236a0-170">Request</span></span>
<span data-ttu-id="236a0-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="236a0-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
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

### <a name="response"></a><span data-ttu-id="236a0-172">応答</span><span class="sxs-lookup"><span data-stu-id="236a0-172">Response</span></span>
<span data-ttu-id="236a0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="236a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



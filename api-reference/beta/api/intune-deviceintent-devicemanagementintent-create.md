---
title: DeviceManagementIntent の作成
description: 新しい deviceManagementIntent オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e4fc01d4219140b215df6d6ebd186d99c830d1b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313315"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="61a3d-103">DeviceManagementIntent の作成</span><span class="sxs-lookup"><span data-stu-id="61a3d-103">Create deviceManagementIntent</span></span>

> <span data-ttu-id="61a3d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61a3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61a3d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61a3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61a3d-106">新しい[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="61a3d-106">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61a3d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="61a3d-107">Prerequisites</span></span>
<span data-ttu-id="61a3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61a3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a3d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61a3d-110">Permission type</span></span>|<span data-ttu-id="61a3d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61a3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61a3d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61a3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61a3d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61a3d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61a3d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61a3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a3d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61a3d-115">Not supported.</span></span>|
|<span data-ttu-id="61a3d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61a3d-116">Application</span></span>|<span data-ttu-id="61a3d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61a3d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61a3d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61a3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="61a3d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61a3d-119">Request headers</span></span>
|<span data-ttu-id="61a3d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61a3d-120">Header</span></span>|<span data-ttu-id="61a3d-121">値</span><span class="sxs-lookup"><span data-stu-id="61a3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61a3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61a3d-122">Authorization</span></span>|<span data-ttu-id="61a3d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="61a3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61a3d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="61a3d-124">Accept</span></span>|<span data-ttu-id="61a3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61a3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61a3d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="61a3d-126">Request body</span></span>
<span data-ttu-id="61a3d-127">要求本文で、deviceManagementIntent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="61a3d-127">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="61a3d-128">次の表に、deviceManagementIntent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="61a3d-128">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="61a3d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61a3d-129">Property</span></span>|<span data-ttu-id="61a3d-130">型</span><span class="sxs-lookup"><span data-stu-id="61a3d-130">Type</span></span>|<span data-ttu-id="61a3d-131">説明</span><span class="sxs-lookup"><span data-stu-id="61a3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61a3d-132">id</span><span class="sxs-lookup"><span data-stu-id="61a3d-132">id</span></span>|<span data-ttu-id="61a3d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="61a3d-133">String</span></span>|<span data-ttu-id="61a3d-134">インテント ID</span><span class="sxs-lookup"><span data-stu-id="61a3d-134">The intent ID</span></span>|
|<span data-ttu-id="61a3d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="61a3d-135">displayName</span></span>|<span data-ttu-id="61a3d-136">String</span><span class="sxs-lookup"><span data-stu-id="61a3d-136">String</span></span>|<span data-ttu-id="61a3d-137">ユーザーが指定した表示名</span><span class="sxs-lookup"><span data-stu-id="61a3d-137">The user given display name</span></span>|
|<span data-ttu-id="61a3d-138">description</span><span class="sxs-lookup"><span data-stu-id="61a3d-138">description</span></span>|<span data-ttu-id="61a3d-139">String</span><span class="sxs-lookup"><span data-stu-id="61a3d-139">String</span></span>|<span data-ttu-id="61a3d-140">ユーザーが指定した説明</span><span class="sxs-lookup"><span data-stu-id="61a3d-140">The user given description</span></span>|
|<span data-ttu-id="61a3d-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="61a3d-141">isAssigned</span></span>|<span data-ttu-id="61a3d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="61a3d-142">Boolean</span></span>|<span data-ttu-id="61a3d-143">目的がユーザーに割り当てられているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="61a3d-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="61a3d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61a3d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="61a3d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61a3d-145">DateTimeOffset</span></span>|<span data-ttu-id="61a3d-146">目的が最後に変更された日時</span><span class="sxs-lookup"><span data-stu-id="61a3d-146">When the intent was last modified</span></span>|
|<span data-ttu-id="61a3d-147">templateId</span><span class="sxs-lookup"><span data-stu-id="61a3d-147">templateId</span></span>|<span data-ttu-id="61a3d-148">String</span><span class="sxs-lookup"><span data-stu-id="61a3d-148">String</span></span>|<span data-ttu-id="61a3d-149">この目的が作成されたテンプレートの ID (存在する場合)</span><span class="sxs-lookup"><span data-stu-id="61a3d-149">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="61a3d-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61a3d-150">roleScopeTagIds</span></span>|<span data-ttu-id="61a3d-151">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="61a3d-151">String collection</span></span>|<span data-ttu-id="61a3d-152">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="61a3d-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="61a3d-153">応答</span><span class="sxs-lookup"><span data-stu-id="61a3d-153">Response</span></span>
<span data-ttu-id="61a3d-154">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="61a3d-154">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a3d-155">例</span><span class="sxs-lookup"><span data-stu-id="61a3d-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="61a3d-156">要求</span><span class="sxs-lookup"><span data-stu-id="61a3d-156">Request</span></span>
<span data-ttu-id="61a3d-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61a3d-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="61a3d-158">応答</span><span class="sxs-lookup"><span data-stu-id="61a3d-158">Response</span></span>
<span data-ttu-id="61a3d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61a3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```







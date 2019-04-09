---
title: devicemanagementintent の作成
description: 新しい devicemanagementintent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c8532ddacd98cd5fcc163544deb663e64cd5390
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522742"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="577e3-103">devicemanagementintent の作成</span><span class="sxs-lookup"><span data-stu-id="577e3-103">Create deviceManagementIntent</span></span>

> <span data-ttu-id="577e3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="577e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="577e3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="577e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="577e3-106">新しい[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="577e3-106">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="577e3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="577e3-107">Prerequisites</span></span>
<span data-ttu-id="577e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="577e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="577e3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="577e3-110">Permission type</span></span>|<span data-ttu-id="577e3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="577e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="577e3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="577e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="577e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="577e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="577e3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="577e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="577e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="577e3-115">Not supported.</span></span>|
|<span data-ttu-id="577e3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="577e3-116">Application</span></span>|<span data-ttu-id="577e3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="577e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="577e3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="577e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="577e3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="577e3-119">Request headers</span></span>
|<span data-ttu-id="577e3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="577e3-120">Header</span></span>|<span data-ttu-id="577e3-121">値</span><span class="sxs-lookup"><span data-stu-id="577e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="577e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="577e3-122">Authorization</span></span>|<span data-ttu-id="577e3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="577e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="577e3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="577e3-124">Accept</span></span>|<span data-ttu-id="577e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="577e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="577e3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="577e3-126">Request body</span></span>
<span data-ttu-id="577e3-127">要求本文で、devicemanagementintent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="577e3-127">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="577e3-128">次の表に、devicemanagementintent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="577e3-128">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="577e3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="577e3-129">Property</span></span>|<span data-ttu-id="577e3-130">型</span><span class="sxs-lookup"><span data-stu-id="577e3-130">Type</span></span>|<span data-ttu-id="577e3-131">説明</span><span class="sxs-lookup"><span data-stu-id="577e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="577e3-132">id</span><span class="sxs-lookup"><span data-stu-id="577e3-132">id</span></span>|<span data-ttu-id="577e3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="577e3-133">String</span></span>|<span data-ttu-id="577e3-134">インテント ID</span><span class="sxs-lookup"><span data-stu-id="577e3-134">The intent ID</span></span>|
|<span data-ttu-id="577e3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="577e3-135">displayName</span></span>|<span data-ttu-id="577e3-136">String</span><span class="sxs-lookup"><span data-stu-id="577e3-136">String</span></span>|<span data-ttu-id="577e3-137">ユーザーが指定した表示名</span><span class="sxs-lookup"><span data-stu-id="577e3-137">The user given display name</span></span>|
|<span data-ttu-id="577e3-138">説明</span><span class="sxs-lookup"><span data-stu-id="577e3-138">description</span></span>|<span data-ttu-id="577e3-139">String</span><span class="sxs-lookup"><span data-stu-id="577e3-139">String</span></span>|<span data-ttu-id="577e3-140">ユーザーが指定した説明</span><span class="sxs-lookup"><span data-stu-id="577e3-140">The user given description</span></span>|
|<span data-ttu-id="577e3-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="577e3-141">isAssigned</span></span>|<span data-ttu-id="577e3-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="577e3-142">Boolean</span></span>|<span data-ttu-id="577e3-143">目的がユーザーに割り当てられているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="577e3-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="577e3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="577e3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="577e3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="577e3-145">DateTimeOffset</span></span>|<span data-ttu-id="577e3-146">目的が最後に変更された日時</span><span class="sxs-lookup"><span data-stu-id="577e3-146">When the intent was last modified</span></span>|
|<span data-ttu-id="577e3-147">templateId</span><span class="sxs-lookup"><span data-stu-id="577e3-147">templateId</span></span>|<span data-ttu-id="577e3-148">文字列</span><span class="sxs-lookup"><span data-stu-id="577e3-148">String</span></span>|<span data-ttu-id="577e3-149">この目的が作成されたテンプレートの ID (存在する場合)</span><span class="sxs-lookup"><span data-stu-id="577e3-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="577e3-150">応答</span><span class="sxs-lookup"><span data-stu-id="577e3-150">Response</span></span>
<span data-ttu-id="577e3-151">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="577e3-151">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="577e3-152">例</span><span class="sxs-lookup"><span data-stu-id="577e3-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="577e3-153">要求</span><span class="sxs-lookup"><span data-stu-id="577e3-153">Request</span></span>
<span data-ttu-id="577e3-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="577e3-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
Content-type: application/json
Content-length: 204

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value"
}
```

### <a name="response"></a><span data-ttu-id="577e3-155">応答</span><span class="sxs-lookup"><span data-stu-id="577e3-155">Response</span></span>
<span data-ttu-id="577e3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="577e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value"
}
```








---
title: devicemanagementintent の更新
description: devicemanagementintent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d73b31e74b56355e46f79ff9c5961f605f2f4fc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523981"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="31e76-103">devicemanagementintent の更新</span><span class="sxs-lookup"><span data-stu-id="31e76-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="31e76-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31e76-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31e76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31e76-106">[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31e76-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31e76-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="31e76-107">Prerequisites</span></span>
<span data-ttu-id="31e76-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31e76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e76-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31e76-110">Permission type</span></span>|<span data-ttu-id="31e76-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31e76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31e76-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31e76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31e76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31e76-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31e76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31e76-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e76-115">Not supported.</span></span>|
|<span data-ttu-id="31e76-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31e76-116">Application</span></span>|<span data-ttu-id="31e76-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31e76-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31e76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="31e76-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31e76-119">Request headers</span></span>
|<span data-ttu-id="31e76-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31e76-120">Header</span></span>|<span data-ttu-id="31e76-121">値</span><span class="sxs-lookup"><span data-stu-id="31e76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31e76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e76-122">Authorization</span></span>|<span data-ttu-id="31e76-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31e76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31e76-124">承諾</span><span class="sxs-lookup"><span data-stu-id="31e76-124">Accept</span></span>|<span data-ttu-id="31e76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31e76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31e76-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="31e76-126">Request body</span></span>
<span data-ttu-id="31e76-127">要求本文で、 [devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31e76-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="31e76-128">次の表に、 [devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31e76-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="31e76-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31e76-129">Property</span></span>|<span data-ttu-id="31e76-130">型</span><span class="sxs-lookup"><span data-stu-id="31e76-130">Type</span></span>|<span data-ttu-id="31e76-131">説明</span><span class="sxs-lookup"><span data-stu-id="31e76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31e76-132">id</span><span class="sxs-lookup"><span data-stu-id="31e76-132">id</span></span>|<span data-ttu-id="31e76-133">文字列</span><span class="sxs-lookup"><span data-stu-id="31e76-133">String</span></span>|<span data-ttu-id="31e76-134">インテント ID</span><span class="sxs-lookup"><span data-stu-id="31e76-134">The intent ID</span></span>|
|<span data-ttu-id="31e76-135">displayName</span><span class="sxs-lookup"><span data-stu-id="31e76-135">displayName</span></span>|<span data-ttu-id="31e76-136">String</span><span class="sxs-lookup"><span data-stu-id="31e76-136">String</span></span>|<span data-ttu-id="31e76-137">ユーザーが指定した表示名</span><span class="sxs-lookup"><span data-stu-id="31e76-137">The user given display name</span></span>|
|<span data-ttu-id="31e76-138">説明</span><span class="sxs-lookup"><span data-stu-id="31e76-138">description</span></span>|<span data-ttu-id="31e76-139">String</span><span class="sxs-lookup"><span data-stu-id="31e76-139">String</span></span>|<span data-ttu-id="31e76-140">ユーザーが指定した説明</span><span class="sxs-lookup"><span data-stu-id="31e76-140">The user given description</span></span>|
|<span data-ttu-id="31e76-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="31e76-141">isAssigned</span></span>|<span data-ttu-id="31e76-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="31e76-142">Boolean</span></span>|<span data-ttu-id="31e76-143">目的がユーザーに割り当てられているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="31e76-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="31e76-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31e76-144">lastModifiedDateTime</span></span>|<span data-ttu-id="31e76-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e76-145">DateTimeOffset</span></span>|<span data-ttu-id="31e76-146">目的が最後に変更された日時</span><span class="sxs-lookup"><span data-stu-id="31e76-146">When the intent was last modified</span></span>|
|<span data-ttu-id="31e76-147">templateId</span><span class="sxs-lookup"><span data-stu-id="31e76-147">templateId</span></span>|<span data-ttu-id="31e76-148">文字列</span><span class="sxs-lookup"><span data-stu-id="31e76-148">String</span></span>|<span data-ttu-id="31e76-149">この目的が作成されたテンプレートの ID (存在する場合)</span><span class="sxs-lookup"><span data-stu-id="31e76-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="31e76-150">応答</span><span class="sxs-lookup"><span data-stu-id="31e76-150">Response</span></span>
<span data-ttu-id="31e76-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31e76-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e76-152">例</span><span class="sxs-lookup"><span data-stu-id="31e76-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="31e76-153">要求</span><span class="sxs-lookup"><span data-stu-id="31e76-153">Request</span></span>
<span data-ttu-id="31e76-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31e76-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
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

### <a name="response"></a><span data-ttu-id="31e76-155">応答</span><span class="sxs-lookup"><span data-stu-id="31e76-155">Response</span></span>
<span data-ttu-id="31e76-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31e76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








---
title: devicemanagementtemplate の更新
description: devicemanagementtemplate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d974ec691b99ecc9f3067f20ab4d2310cbe27d23
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466568"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="53c91-103">devicemanagementtemplate の更新</span><span class="sxs-lookup"><span data-stu-id="53c91-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="53c91-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53c91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c91-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53c91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c91-106">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="53c91-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c91-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="53c91-107">Prerequisites</span></span>
<span data-ttu-id="53c91-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c91-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53c91-110">Permission type</span></span>|<span data-ttu-id="53c91-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53c91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c91-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53c91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53c91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53c91-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53c91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c91-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53c91-115">Not supported.</span></span>|
|<span data-ttu-id="53c91-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53c91-116">Application</span></span>|<span data-ttu-id="53c91-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53c91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c91-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53c91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="53c91-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53c91-119">Request headers</span></span>
|<span data-ttu-id="53c91-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53c91-120">Header</span></span>|<span data-ttu-id="53c91-121">値</span><span class="sxs-lookup"><span data-stu-id="53c91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53c91-122">Authorization</span></span>|<span data-ttu-id="53c91-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="53c91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c91-124">承諾</span><span class="sxs-lookup"><span data-stu-id="53c91-124">Accept</span></span>|<span data-ttu-id="53c91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53c91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c91-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53c91-126">Request body</span></span>
<span data-ttu-id="53c91-127">要求本文で、 [devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53c91-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="53c91-128">次の表に、 [devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53c91-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="53c91-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53c91-129">Property</span></span>|<span data-ttu-id="53c91-130">型</span><span class="sxs-lookup"><span data-stu-id="53c91-130">Type</span></span>|<span data-ttu-id="53c91-131">説明</span><span class="sxs-lookup"><span data-stu-id="53c91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c91-132">id</span><span class="sxs-lookup"><span data-stu-id="53c91-132">id</span></span>|<span data-ttu-id="53c91-133">String</span><span class="sxs-lookup"><span data-stu-id="53c91-133">String</span></span>|<span data-ttu-id="53c91-134">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="53c91-134">The template ID</span></span>|
|<span data-ttu-id="53c91-135">displayName</span><span class="sxs-lookup"><span data-stu-id="53c91-135">displayName</span></span>|<span data-ttu-id="53c91-136">String</span><span class="sxs-lookup"><span data-stu-id="53c91-136">String</span></span>|<span data-ttu-id="53c91-137">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="53c91-137">The template's display name</span></span>|
|<span data-ttu-id="53c91-138">説明</span><span class="sxs-lookup"><span data-stu-id="53c91-138">description</span></span>|<span data-ttu-id="53c91-139">String</span><span class="sxs-lookup"><span data-stu-id="53c91-139">String</span></span>|<span data-ttu-id="53c91-140">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="53c91-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="53c91-141">応答</span><span class="sxs-lookup"><span data-stu-id="53c91-141">Response</span></span>
<span data-ttu-id="53c91-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53c91-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c91-143">例</span><span class="sxs-lookup"><span data-stu-id="53c91-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c91-144">要求</span><span class="sxs-lookup"><span data-stu-id="53c91-144">Request</span></span>
<span data-ttu-id="53c91-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53c91-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="53c91-146">応答</span><span class="sxs-lookup"><span data-stu-id="53c91-146">Response</span></span>
<span data-ttu-id="53c91-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53c91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```






---
title: securityBaselineTemplate の更新
description: securityBaselineTemplate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f2cb66df449dc8586ef3fb3f822fadf62891902
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800610"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="5a8a0-103">securityBaselineTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="5a8a0-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="5a8a0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a8a0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a8a0-106">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a8a0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5a8a0-107">Prerequisites</span></span>
<span data-ttu-id="5a8a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a8a0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a8a0-110">Permission type</span></span>|<span data-ttu-id="5a8a0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a8a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a8a0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a8a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a8a0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a8a0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a8a0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a8a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a8a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-115">Not supported.</span></span>|
|<span data-ttu-id="5a8a0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a8a0-116">Application</span></span>|<span data-ttu-id="5a8a0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a8a0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a8a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="5a8a0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a8a0-119">Request headers</span></span>
|<span data-ttu-id="5a8a0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a8a0-120">Header</span></span>|<span data-ttu-id="5a8a0-121">値</span><span class="sxs-lookup"><span data-stu-id="5a8a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a8a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a8a0-122">Authorization</span></span>|<span data-ttu-id="5a8a0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a8a0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5a8a0-124">Accept</span></span>|<span data-ttu-id="5a8a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a8a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a8a0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a8a0-126">Request body</span></span>
<span data-ttu-id="5a8a0-127">要求本文で、 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="5a8a0-128">次の表に、 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="5a8a0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a8a0-129">Property</span></span>|<span data-ttu-id="5a8a0-130">型</span><span class="sxs-lookup"><span data-stu-id="5a8a0-130">Type</span></span>|<span data-ttu-id="5a8a0-131">説明</span><span class="sxs-lookup"><span data-stu-id="5a8a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a8a0-132">id</span><span class="sxs-lookup"><span data-stu-id="5a8a0-132">id</span></span>|<span data-ttu-id="5a8a0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="5a8a0-133">String</span></span>|<span data-ttu-id="5a8a0-134">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID</span><span class="sxs-lookup"><span data-stu-id="5a8a0-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="5a8a0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5a8a0-135">displayName</span></span>|<span data-ttu-id="5a8a0-136">String</span><span class="sxs-lookup"><span data-stu-id="5a8a0-136">String</span></span>|<span data-ttu-id="5a8a0-137">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="5a8a0-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="5a8a0-138">説明</span><span class="sxs-lookup"><span data-stu-id="5a8a0-138">description</span></span>|<span data-ttu-id="5a8a0-139">String</span><span class="sxs-lookup"><span data-stu-id="5a8a0-139">String</span></span>|<span data-ttu-id="5a8a0-140">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="5a8a0-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5a8a0-141">応答</span><span class="sxs-lookup"><span data-stu-id="5a8a0-141">Response</span></span>
<span data-ttu-id="5a8a0-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a8a0-143">例</span><span class="sxs-lookup"><span data-stu-id="5a8a0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a8a0-144">要求</span><span class="sxs-lookup"><span data-stu-id="5a8a0-144">Request</span></span>
<span data-ttu-id="5a8a0-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="5a8a0-146">応答</span><span class="sxs-lookup"><span data-stu-id="5a8a0-146">Response</span></span>
<span data-ttu-id="5a8a0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a8a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```






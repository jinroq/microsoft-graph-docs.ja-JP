---
title: securityBaselineTemplate を作成する
description: 新しい securityBaselineTemplate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d6f48f0fdb95f2d88f6af5f62975792453367d9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773491"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="26954-103">securityBaselineTemplate を作成する</span><span class="sxs-lookup"><span data-stu-id="26954-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="26954-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26954-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26954-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26954-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26954-106">新しい[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26954-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26954-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="26954-107">Prerequisites</span></span>
<span data-ttu-id="26954-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26954-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26954-110">Permission type</span></span>|<span data-ttu-id="26954-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26954-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26954-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26954-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26954-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26954-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26954-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26954-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26954-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26954-115">Not supported.</span></span>|
|<span data-ttu-id="26954-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26954-116">Application</span></span>|<span data-ttu-id="26954-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26954-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26954-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26954-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="26954-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26954-119">Request headers</span></span>
|<span data-ttu-id="26954-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26954-120">Header</span></span>|<span data-ttu-id="26954-121">値</span><span class="sxs-lookup"><span data-stu-id="26954-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26954-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26954-122">Authorization</span></span>|<span data-ttu-id="26954-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="26954-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26954-124">承諾</span><span class="sxs-lookup"><span data-stu-id="26954-124">Accept</span></span>|<span data-ttu-id="26954-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26954-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26954-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="26954-126">Request body</span></span>
<span data-ttu-id="26954-127">要求本文で、securityBaselineTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26954-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="26954-128">次の表に、securityBaselineTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26954-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="26954-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26954-129">Property</span></span>|<span data-ttu-id="26954-130">型</span><span class="sxs-lookup"><span data-stu-id="26954-130">Type</span></span>|<span data-ttu-id="26954-131">説明</span><span class="sxs-lookup"><span data-stu-id="26954-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26954-132">id</span><span class="sxs-lookup"><span data-stu-id="26954-132">id</span></span>|<span data-ttu-id="26954-133">文字列</span><span class="sxs-lookup"><span data-stu-id="26954-133">String</span></span>|<span data-ttu-id="26954-134">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID</span><span class="sxs-lookup"><span data-stu-id="26954-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="26954-135">displayName</span><span class="sxs-lookup"><span data-stu-id="26954-135">displayName</span></span>|<span data-ttu-id="26954-136">String</span><span class="sxs-lookup"><span data-stu-id="26954-136">String</span></span>|<span data-ttu-id="26954-137">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="26954-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="26954-138">説明</span><span class="sxs-lookup"><span data-stu-id="26954-138">description</span></span>|<span data-ttu-id="26954-139">String</span><span class="sxs-lookup"><span data-stu-id="26954-139">String</span></span>|<span data-ttu-id="26954-140">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="26954-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="26954-141">応答</span><span class="sxs-lookup"><span data-stu-id="26954-141">Response</span></span>
<span data-ttu-id="26954-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26954-142">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26954-143">例</span><span class="sxs-lookup"><span data-stu-id="26954-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="26954-144">要求</span><span class="sxs-lookup"><span data-stu-id="26954-144">Request</span></span>
<span data-ttu-id="26954-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26954-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="26954-146">応答</span><span class="sxs-lookup"><span data-stu-id="26954-146">Response</span></span>
<span data-ttu-id="26954-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26954-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```






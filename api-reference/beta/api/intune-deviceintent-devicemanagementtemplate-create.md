---
title: devicemanagementtemplate の作成
description: 新しい devicemanagementtemplate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23c86d654d229c4932a9e5b7d86d980416637b2a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807925"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="ebb52-103">devicemanagementtemplate の作成</span><span class="sxs-lookup"><span data-stu-id="ebb52-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="ebb52-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebb52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb52-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebb52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb52-106">新しい[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ebb52-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebb52-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebb52-107">Prerequisites</span></span>
<span data-ttu-id="ebb52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebb52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebb52-110">Permission type</span></span>|<span data-ttu-id="ebb52-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebb52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebb52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebb52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebb52-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb52-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebb52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebb52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebb52-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebb52-115">Not supported.</span></span>|
|<span data-ttu-id="ebb52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebb52-116">Application</span></span>|<span data-ttu-id="ebb52-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebb52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebb52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebb52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="ebb52-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebb52-119">Request headers</span></span>
|<span data-ttu-id="ebb52-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebb52-120">Header</span></span>|<span data-ttu-id="ebb52-121">値</span><span class="sxs-lookup"><span data-stu-id="ebb52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebb52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebb52-122">Authorization</span></span>|<span data-ttu-id="ebb52-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebb52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebb52-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ebb52-124">Accept</span></span>|<span data-ttu-id="ebb52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebb52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebb52-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebb52-126">Request body</span></span>
<span data-ttu-id="ebb52-127">要求本文で、devicemanagementtemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebb52-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="ebb52-128">次の表に、devicemanagementtemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ebb52-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="ebb52-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb52-129">Property</span></span>|<span data-ttu-id="ebb52-130">型</span><span class="sxs-lookup"><span data-stu-id="ebb52-130">Type</span></span>|<span data-ttu-id="ebb52-131">説明</span><span class="sxs-lookup"><span data-stu-id="ebb52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb52-132">id</span><span class="sxs-lookup"><span data-stu-id="ebb52-132">id</span></span>|<span data-ttu-id="ebb52-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ebb52-133">String</span></span>|<span data-ttu-id="ebb52-134">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="ebb52-134">The template ID</span></span>|
|<span data-ttu-id="ebb52-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ebb52-135">displayName</span></span>|<span data-ttu-id="ebb52-136">String</span><span class="sxs-lookup"><span data-stu-id="ebb52-136">String</span></span>|<span data-ttu-id="ebb52-137">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="ebb52-137">The template's display name</span></span>|
|<span data-ttu-id="ebb52-138">説明</span><span class="sxs-lookup"><span data-stu-id="ebb52-138">description</span></span>|<span data-ttu-id="ebb52-139">String</span><span class="sxs-lookup"><span data-stu-id="ebb52-139">String</span></span>|<span data-ttu-id="ebb52-140">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="ebb52-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="ebb52-141">応答</span><span class="sxs-lookup"><span data-stu-id="ebb52-141">Response</span></span>
<span data-ttu-id="ebb52-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebb52-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebb52-143">例</span><span class="sxs-lookup"><span data-stu-id="ebb52-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebb52-144">要求</span><span class="sxs-lookup"><span data-stu-id="ebb52-144">Request</span></span>
<span data-ttu-id="ebb52-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebb52-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ebb52-146">応答</span><span class="sxs-lookup"><span data-stu-id="ebb52-146">Response</span></span>
<span data-ttu-id="ebb52-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebb52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```






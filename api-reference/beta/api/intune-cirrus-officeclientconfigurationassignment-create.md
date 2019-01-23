---
title: OfficeClientConfigurationAssignment を作成します。
description: ターゲット グループを既存のポリシーに追加します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1f09ba2dfabf85501120cb2099373e5664deb08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425198"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="60d99-103">OfficeClientConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="60d99-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="60d99-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60d99-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60d99-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60d99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60d99-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60d99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60d99-107">ターゲット グループを既存のポリシーに追加します。</span><span class="sxs-lookup"><span data-stu-id="60d99-107">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60d99-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="60d99-108">Prerequisites</span></span>
<span data-ttu-id="60d99-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60d99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d99-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60d99-111">Permission type</span></span>|<span data-ttu-id="60d99-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60d99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60d99-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60d99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60d99-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d99-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60d99-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60d99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60d99-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60d99-116">Not supported.</span></span>|
|<span data-ttu-id="60d99-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60d99-117">Application</span></span>|<span data-ttu-id="60d99-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60d99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60d99-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60d99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="60d99-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60d99-120">Request headers</span></span>
|<span data-ttu-id="60d99-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60d99-121">Header</span></span>|<span data-ttu-id="60d99-122">値</span><span class="sxs-lookup"><span data-stu-id="60d99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60d99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60d99-123">Authorization</span></span>|<span data-ttu-id="60d99-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="60d99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60d99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60d99-125">Accept</span></span>|<span data-ttu-id="60d99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60d99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d99-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="60d99-127">Request body</span></span>
<span data-ttu-id="60d99-128">要求の本文に officeClientConfigurationAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="60d99-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="60d99-129">次の表は、officeClientConfigurationAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="60d99-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="60d99-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60d99-130">Property</span></span>|<span data-ttu-id="60d99-131">型</span><span class="sxs-lookup"><span data-stu-id="60d99-131">Type</span></span>|<span data-ttu-id="60d99-132">説明</span><span class="sxs-lookup"><span data-stu-id="60d99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60d99-133">id</span><span class="sxs-lookup"><span data-stu-id="60d99-133">id</span></span>|<span data-ttu-id="60d99-134">String</span><span class="sxs-lookup"><span data-stu-id="60d99-134">String</span></span>|<span data-ttu-id="60d99-135">OfficeConfigurationAssignment の id です。</span><span class="sxs-lookup"><span data-stu-id="60d99-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="60d99-136">target</span><span class="sxs-lookup"><span data-stu-id="60d99-136">target</span></span>|[<span data-ttu-id="60d99-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="60d99-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="60d99-138">Admin によって定義されているターゲットの割り当て</span><span class="sxs-lookup"><span data-stu-id="60d99-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="60d99-139">応答</span><span class="sxs-lookup"><span data-stu-id="60d99-139">Response</span></span>
<span data-ttu-id="60d99-140">かどうかは成功すると、このメソッドが返されます、`200 Created`応答コードおよび応答の本文に[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="60d99-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60d99-141">例</span><span class="sxs-lookup"><span data-stu-id="60d99-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="60d99-142">要求</span><span class="sxs-lookup"><span data-stu-id="60d99-142">Request</span></span>
<span data-ttu-id="60d99-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60d99-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="60d99-144">応答</span><span class="sxs-lookup"><span data-stu-id="60d99-144">Response</span></span>
<span data-ttu-id="60d99-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60d99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```




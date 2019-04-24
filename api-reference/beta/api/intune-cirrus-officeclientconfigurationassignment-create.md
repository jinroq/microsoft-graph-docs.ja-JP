---
title: officeClientConfigurationAssignment を作成する
description: 既存のポリシーにターゲットグループを追加します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e646b70ea3e18a79aaee5b4129e54da833c5c4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483825"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="be5ac-103">officeClientConfigurationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="be5ac-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="be5ac-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be5ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be5ac-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be5ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be5ac-106">既存のポリシーにターゲットグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="be5ac-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be5ac-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="be5ac-107">Prerequisites</span></span>
<span data-ttu-id="be5ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5ac-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be5ac-110">Permission type</span></span>|<span data-ttu-id="be5ac-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="be5ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be5ac-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be5ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be5ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be5ac-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be5ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be5ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be5ac-115">Not supported.</span></span>|
|<span data-ttu-id="be5ac-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be5ac-116">Application</span></span>|<span data-ttu-id="be5ac-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be5ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be5ac-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="be5ac-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be5ac-119">Request headers</span></span>
|<span data-ttu-id="be5ac-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be5ac-120">Header</span></span>|<span data-ttu-id="be5ac-121">値</span><span class="sxs-lookup"><span data-stu-id="be5ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be5ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be5ac-122">Authorization</span></span>|<span data-ttu-id="be5ac-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="be5ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be5ac-124">承諾</span><span class="sxs-lookup"><span data-stu-id="be5ac-124">Accept</span></span>|<span data-ttu-id="be5ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be5ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be5ac-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="be5ac-126">Request body</span></span>
<span data-ttu-id="be5ac-127">要求本文で、officeClientConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="be5ac-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="be5ac-128">次の表に、officeClientConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="be5ac-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="be5ac-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be5ac-129">Property</span></span>|<span data-ttu-id="be5ac-130">型</span><span class="sxs-lookup"><span data-stu-id="be5ac-130">Type</span></span>|<span data-ttu-id="be5ac-131">説明</span><span class="sxs-lookup"><span data-stu-id="be5ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5ac-132">id</span><span class="sxs-lookup"><span data-stu-id="be5ac-132">id</span></span>|<span data-ttu-id="be5ac-133">String</span><span class="sxs-lookup"><span data-stu-id="be5ac-133">String</span></span>|<span data-ttu-id="be5ac-134">OfficeConfigurationAssignment の Id。</span><span class="sxs-lookup"><span data-stu-id="be5ac-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="be5ac-135">target</span><span class="sxs-lookup"><span data-stu-id="be5ac-135">target</span></span>|[<span data-ttu-id="be5ac-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="be5ac-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="be5ac-137">管理者によって定義されたターゲットの割り当て。</span><span class="sxs-lookup"><span data-stu-id="be5ac-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="be5ac-138">応答</span><span class="sxs-lookup"><span data-stu-id="be5ac-138">Response</span></span>
<span data-ttu-id="be5ac-139">成功した場合、このメソッド`200 Created`は応答コードと、応答本文で[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be5ac-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be5ac-140">例</span><span class="sxs-lookup"><span data-stu-id="be5ac-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="be5ac-141">要求</span><span class="sxs-lookup"><span data-stu-id="be5ac-141">Request</span></span>
<span data-ttu-id="be5ac-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be5ac-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be5ac-143">応答</span><span class="sxs-lookup"><span data-stu-id="be5ac-143">Response</span></span>
<span data-ttu-id="be5ac-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be5ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: GroupPolicyPresentationTextBox を作成します。
description: 新しい groupPolicyPresentationTextBox オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20a34e2288541fe948464b1410398138316943a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430489"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="cc330-103">GroupPolicyPresentationTextBox を作成します。</span><span class="sxs-lookup"><span data-stu-id="cc330-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="cc330-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc330-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc330-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc330-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc330-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc330-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc330-107">新しい[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc330-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc330-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc330-108">Prerequisites</span></span>
<span data-ttu-id="cc330-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc330-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc330-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc330-111">Permission type</span></span>|<span data-ttu-id="cc330-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc330-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc330-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc330-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc330-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc330-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc330-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc330-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc330-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc330-116">Not supported.</span></span>|
|<span data-ttu-id="cc330-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc330-117">Application</span></span>|<span data-ttu-id="cc330-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc330-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc330-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc330-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="cc330-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc330-120">Request headers</span></span>
|<span data-ttu-id="cc330-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc330-121">Header</span></span>|<span data-ttu-id="cc330-122">値</span><span class="sxs-lookup"><span data-stu-id="cc330-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc330-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc330-123">Authorization</span></span>|<span data-ttu-id="cc330-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc330-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc330-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc330-125">Accept</span></span>|<span data-ttu-id="cc330-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc330-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc330-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc330-127">Request body</span></span>
<span data-ttu-id="cc330-128">要求の本文に groupPolicyPresentationTextBox オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc330-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="cc330-129">次の表は、groupPolicyPresentationTextBox を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc330-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="cc330-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc330-130">Property</span></span>|<span data-ttu-id="cc330-131">型</span><span class="sxs-lookup"><span data-stu-id="cc330-131">Type</span></span>|<span data-ttu-id="cc330-132">説明</span><span class="sxs-lookup"><span data-stu-id="cc330-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc330-133">label</span><span class="sxs-lookup"><span data-stu-id="cc330-133">label</span></span>|<span data-ttu-id="cc330-134">String</span><span class="sxs-lookup"><span data-stu-id="cc330-134">String</span></span>|<span data-ttu-id="cc330-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="cc330-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cc330-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="cc330-136">The default value is empty.</span></span> <span data-ttu-id="cc330-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cc330-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc330-138">id</span><span class="sxs-lookup"><span data-stu-id="cc330-138">id</span></span>|<span data-ttu-id="cc330-139">String</span><span class="sxs-lookup"><span data-stu-id="cc330-139">String</span></span>|<span data-ttu-id="cc330-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cc330-140">Key of the entity.</span></span> <span data-ttu-id="cc330-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cc330-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc330-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc330-142">lastModifiedDateTime</span></span>|<span data-ttu-id="cc330-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc330-143">DateTimeOffset</span></span>|<span data-ttu-id="cc330-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="cc330-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="cc330-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cc330-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc330-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="cc330-146">defaultValue</span></span>|<span data-ttu-id="cc330-147">文字列</span><span class="sxs-lookup"><span data-stu-id="cc330-147">String</span></span>|<span data-ttu-id="cc330-148">テキスト ボックスに表示される既定の文字列をローカライズします。</span><span class="sxs-lookup"><span data-stu-id="cc330-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="cc330-149">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="cc330-149">The default value is empty.</span></span>|
|<span data-ttu-id="cc330-150">必須</span><span class="sxs-lookup"><span data-stu-id="cc330-150">required</span></span>|<span data-ttu-id="cc330-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc330-151">Boolean</span></span>|<span data-ttu-id="cc330-152">テキスト ボックスに値を入力するための要件。</span><span class="sxs-lookup"><span data-stu-id="cc330-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="cc330-153">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="cc330-153">Default value is false.</span></span>|
|<span data-ttu-id="cc330-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="cc330-154">maxLength</span></span>|<span data-ttu-id="cc330-155">Int64</span><span class="sxs-lookup"><span data-stu-id="cc330-155">Int64</span></span>|<span data-ttu-id="cc330-156">テキスト文字の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="cc330-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="cc330-157">1023 を既定値には。</span><span class="sxs-lookup"><span data-stu-id="cc330-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="cc330-158">応答</span><span class="sxs-lookup"><span data-stu-id="cc330-158">Response</span></span>
<span data-ttu-id="cc330-159">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cc330-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc330-160">例</span><span class="sxs-lookup"><span data-stu-id="cc330-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc330-161">要求</span><span class="sxs-lookup"><span data-stu-id="cc330-161">Request</span></span>
<span data-ttu-id="cc330-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc330-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="cc330-163">応答</span><span class="sxs-lookup"><span data-stu-id="cc330-163">Response</span></span>
<span data-ttu-id="cc330-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc330-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```





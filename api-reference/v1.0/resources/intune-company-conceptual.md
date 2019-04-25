---
title: microsoft Intune での会社の使用条件-microsoft Graph API
description: 会社の使用条件をサポートする Intune (REST) エンドポイントの Microsoft graph API を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 3de3cdf4ac55177bceb56e59743d0bef9bd4cb50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523974"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune の会社の使用条件

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。 ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。

さまざまな使用条件を含む複数のポリシーを作成して展開することができます。 同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。

次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。

- [使用条件](intune-companyterms-termsandconditions.md)
- [使用条件の承認状態](intune-companyterms-termsandconditionsacceptancestatus.md)
- [使用条件の割り当て](intune-companyterms-termsandconditionsassignment.md)

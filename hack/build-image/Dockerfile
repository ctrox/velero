# Copyright 2018 the Heptio Ark contributors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM gcr.io/heptio-images/golang:1.9-alpine3.6

RUN mkdir -p /go/src/k8s.io && \
    cd /go/src/k8s.io && \
    git clone -b kubernetes-1.9.0 https://github.com/kubernetes/code-generator && \
    git clone -b kubernetes-1.9.0 https://github.com/kubernetes/apimachinery && \
    echo chmod -R a+w /go